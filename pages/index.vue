<template>
  <div>
	  <h1>{{title}}</h1>
	  <img src="@/assets/img/feline.jpg" alt="">
  </div>
</template>

<script>
export default {
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
			hid: 'description',
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

