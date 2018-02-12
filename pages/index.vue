<template>
  <div>
	  <h1>{{title}}</h1>
	  <img src="@/assets/img/feline.jpg" alt="">
  </div>
</template>

<script>
export default {
	// middleware: 'authenticated',
	 layout (context) {
    return 'blog'
  },
  data () {
    return {
      title: 'Hello teste World!'
    }
  },
  head () {
    return {
      title: this.title,
      meta: [
        {
			hid: 'description teste',
			name: 'description',
			content: 'My custom description',

			 },
			 {	titleTemplate: 'é aqui'

			 },
			 {
				  htmlAttrs: {
				foo: 'bar',
				amp: undefined

			 }
			 }
	  ]

    }
  },
}
</script>

