<!-- https://jsfiddle.net/2qjvzh0m/5/
https://www.digitalocean.com/community/tutorials/vuejs-vue-modal-component -->
<template>
  <!-- <transition name="modal-fade">
    <div class="modal-backdrop">
      <div
        class="modal"
        role="dialog"
        aria-labelledby="modalTitle"
        aria-describedby="modalDescription"
      >
        <header class="modal-header" id="modalTitle">
          <slot name="header">
            This is the default tile!
            <button
              type="button"
              class="btn-close"
              @click="close"
              aria-label="Close modal"
            >x</button>
          </slot>
        </header>
        <section class="modal-body" id="modalDescription">
          <slot name="body">I'm the default body!</slot>
        </section>
        <footer class="modal-footer">
          <slot name="footer">
            I'm the default footer!
            <button
              type="button"
              class="btn-green"
              @click="close"
              aria-label="Close modal"
            >Close me!</button>
          </slot>
        </footer>
      </div>
    </div>
  </transition>-->

  <transition name="modal-fade">
    <div class="modal-backdrop">
      <div
        class="modal"
        role="dialog"
        aria-labelledby="modalTitle"
        aria-describedby="modalDescription"
      >
        <div class="modal-header" id="modalTitle">
          <slot name="header">Im a header!</slot>
          <button type="button" class="btn-close" @click="close">x</button>
        </div>

        <div class="modal-body" id="modalDescription">
          <slot name="body">Im a body</slot>
        </div>

        <div class="modal-footer">
          <slot name="footer">Im a footer</slot>
          <button type="button" class="btn-green" @click="close">close me</button>
        </div>
      </div>
    </div>
  </transition>
</template>


  <!-- <div>
    <div class="flex items-center justify-center h-64">
      <button
        class="modal-button bg-teal-200 p-3 rounded-lg text-teal-900 hover:bg-teal-300"
      >Blast off</button>
    </div>

    <div
      class="modal opacity-0 pointer-events-none absolute w-full h-full top-0 left-0 flex items-center justify-center"
    >
      <div
        class="modal-overlay absolute w-full h-full bg-black opacity-25 top-0 left-0 cursor-pointer"
      ></div>
      <div
        class="absolute w-1/2 h-32 bg-white rounded-sm shadow-lg flex items-center justify-center text-2xl"
      >🚀</div>
    </div>
  </div>-->
</template>

<script>
export default {
  name: 'Modal',
  methods: {
    close() {
      this.$emit('close')
    }
  }
}

// export default {
//   name: 'Modal',

//   methods: {
//     close() {
//       this.$emit('close')
//     }
//   }
// }

// const button = document.querySelector('.modal-button')
// button.addEventListener('click', toggleModal)

// const overlay = document.querySelector('.modal-overlay')
// overlay.addEventListener('click', toggleModal)

// function toggleModal() {
//   const modal = document.querySelector('.modal')
//   modal.classList.toggle('opacity-0')
//   modal.classList.toggle('pointer-events-none')
// }
</script>

<style scoped>
.modal-backdrop {
  position: fixed;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  background-color: rgba(0, 0, 0, 0.3);
  display: flex;
  justify-content: center;
  align-items: center;
}

.modal {
  background: #ffffff;
  box-shadow: 2px 2px 20px 1px;
  overflow-x: auto;
  display: flex;
  flex-direction: column;
}

.modal-header,
.modal-footer {
  padding: 15px;
  display: flex;
}

.modal-header {
  border-bottom: 1px solid #eeeeee;
  color: #4aae9b;
  justify-content: space-between;
}

.modal-footer {
  border-top: 1px solid #eeeeee;
  justify-content: flex-end;
}

.modal-body {
  position: relative;
  padding: 20px 10px;
}

.btn-close {
  border: none;
  font-size: 20px;
  padding: 20px;
  cursor: pointer;
  font-weight: bold;
  color: #4aae9b;
  background: transparent;
}

.btn-green {
  color: white;
  background: #4aae9b;
  border: 1px solid #4aae9b;
  border-radius: 2px;
}

.modal-fade-enter,
.modal-fade-leave-active {
  opacity: 0;
}

.modal-fade-enter-active,
.modal-fade-leave-active {
  transition: opacity 0.5s ease;
}
/* button {
  border: 2px solid black;
  color: black;
} */
</style>
