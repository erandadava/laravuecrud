<template>
    <div class="container">
        <div class="container">
        	<nav class="navbar navbar-expand-sm bg-dark navbar-dark">
				<ul class="navbar-nav">
					<li class="nav-item">
						<router-link to="/" class="nav-link"> Home </router-link>
					</li>
					<li>
						<router-link to="/create" class="nav-link"> Create Posts </router-link>
					</li>
					<li>
						<router-link to="/posts" class="nav-link"> Posts </router-link>
					</li>
				</ul>
        	</nav> <br />
<!--        <transition name="fade">
                <router-view></router-view>
            </transition> -->
			<transition>
                <router-view></router-view>
            </transition>
        </div>
    </div>
</template>

<style>
    .fade-enter-active, .fade-leave-active {
      transition: opacity .5s
    }
    .fade-enter, .fade-leave-active {
      opacity: 0
    }
</style>

<script>

    export default{
    }
 </script>