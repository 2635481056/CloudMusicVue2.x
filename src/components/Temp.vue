<template>
	<div id=""  >
		<ul>
			<li v-for="m,index in msg" :key="index">{{index}} {{m.songName}}</li>
	
		</ul>
	</div>
</template>

<script>
	export default{
		name:'Temp',
		props:{
			msg:{
				type:Array,
				default(){
					return [
					{songName:"name1" , singerName:"name1"},
					{songName:"name2" , singerName:"name3"},
					{songName:"name3" , singerName:"name4"},
					{songName:"name4" , singerName:"name5"},
				]}
			}
		}
	}
	
</script>

<style>
	*{
		color: white !important;
	}
	
</style>
