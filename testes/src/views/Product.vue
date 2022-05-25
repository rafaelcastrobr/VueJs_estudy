    <template>
      <div>
        Product Page
      </div>
      <span>
          Looking for Product: {{ this.$route.params.id }} 
      </span>
    </template>

    <script>
    export default {
      name: 'ProductVue'
    }
    </script>