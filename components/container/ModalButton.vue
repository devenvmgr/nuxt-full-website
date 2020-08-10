<template>
  <div>
    <button type="button" class="btn" @click="showModal">Open Modal!</button>

    <Modal v-show="isModalVisible" @close="closeModal">
      <template v-slot:header>No Im am the eye hole!</template>
      <template v-slot:body>Check out my body</template>
      <template v-slot:footer>Thi sis the pop up footer</template>
    </Modal>
  </div>
</template>

<script>
import Modal from '../bits/Modal.vue'

export default {
  name: 'ModalButton',
  components: {
    Modal
  },
  data() {
    return {
      isModalVisible: false
    }
  },
  methods: {
    showModal() {
      this.isModalVisible = true
    },
    closeModal() {
      this.isModalVisible = false
    }
  }
}
// export default {
//   name: 'ModalButton',
//   components: {
//     Modal
//   },
//   data() {
//     return {
//       isModalVisible: false
//     }
//   },
//   methods: {
//     showModal() {
//       this.isModalVisible = true
//     },
//     closeModal() {
//       this.isModalVisible = false
//     }
//   }
// }
</script>

<style>
</style>
