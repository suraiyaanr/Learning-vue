<template>
	<span>
		<div>
			<p>{{ message }}</p>
              <button v-on:click="reverseMessage" class="btn btn-block btn-success">Click Reverse String</button>
          
		</div>
	</span>
</template>

<script>  
export default {
		data() {
			return {
				message: 'Saya sedang belajar VueJS'
			}
		},
		methods: {
			reverseMessage: function () {
			this.message = this.message.split('').reverse().join('')
			}
  }
	}
</script>
