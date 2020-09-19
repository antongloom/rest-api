<template lang="pug">
.modal
  h2 REST API
  v-form(ref='form' class="modal-form")
   .modal-input
    v-text-field(v-model='name' label='Имя')
   .modal-input 
    v-text-field(v-model='value' label='Значение')
   v-btn(color='blue' @click='submit')
      | Отправить
  .modal-content
   .modal-title Name
   .modal-description value
   .modal-btns
    v-btn(color='blue' @click='cansel') Отменить
    v-btn(color='red' @click='delet') Удалить
</template>

<script>
// @ is an alias to /src

export default {
	name: 'Home',
	data () {
		return {
			name: '',
      vlaue: '',
		}
	}
}
</script>


<style lang="less">
.modal {
	width: 700px;
	margin: 0 auto;
	margin-top: 50px
}
.modal-form {
	display: flex;
	justify-content: space-between;
}

.modal-input {
	width: 220px;
}

.modal-content {
	border: 1px solid green;
	padding: 20px;
}
.modal-title {
	font-size: 20px;
	font-weight: 500;
}
.modal-btns {
	margin-top: 20px;
	width: 240px;
	display: flex;
	justify-content: space-between;
}
</style>
