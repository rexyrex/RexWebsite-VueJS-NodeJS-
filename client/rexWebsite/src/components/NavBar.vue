<template>
<div id="NavBar">
	<nav class="navbar navbar-default">
		<div class="container-fluid">
			
			<div class="navbar-header">
				<button type="button" class="navbar-toggle" data-toggle="collapse" data-target="#bs-example-navbar-collapse-1"> <span class="sr-only">Toggle navigation</span> <span class="icon-bar"></span> <span class="icon-bar"></span> <span class="icon-bar"></span> </button>
			</div>
			
			<div class="navbar-collapse collapse">
				
				<ul class="nav navbar-nav">
					<li><a href="#" v-on:click="goTo('/')">Home</a></li>
					<li class="active" v-on:click="goTo('/about')"><a href="#">About</a></li>
					<li class="dropdown">
						<a href="#" class="dropdown-toggle" data-toggle="dropdown">More Pages <b class="caret"></b></a>
						<ul class="dropdown-menu">
							<li><a href="#">Rex</a></li>
							<li><a href="#">Zamboni</a></li>
							<li><a href="#">Hooly</a></li>
						</ul>
					</li>
					<li><a href="#">Blog</a></li>
				</ul>
			
			</div><!--/.nav-collapse -->			
		</div>	
	</nav>
</div>
</template>

<script>
export default {
  name: 'NavBar',
  data () {
    return {

    }
  },
  methods: {
      goTo: function(dest){
          this.$router.push(dest);
      }
  }
}
</script>