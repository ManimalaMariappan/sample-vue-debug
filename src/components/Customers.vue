<template>
  <div class="customers container">
    <h1 class="page-header">Manage Customers</h1>
    <p>yvt</p>
  </div>
</template>

<script>
export default {
  name: 'Customers',
  data () {
    return {
      customers: []     
    }
  },
  methods: {
    fetchCustomers: function(){
      console.log('success');
      this.$http.get('https://jsonplaceholder.typicode.com/posts/')
      .then(function(response){
        console.log(response.body);
      })
      .catch(function (resp){
        console.log(resp);
      });
    },
    fetchcus: function () {
      console.log('success');
    }
  },
  mounted () {
    console.log('created');
    this.fetchcus();
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
