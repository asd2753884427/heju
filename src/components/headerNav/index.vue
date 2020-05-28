<template>
	<ul>
		<li v-for="(ar,index) in navData" :key="index"><router-link :class="{active:ar.buer}" :to="ar.to">{{ar.name}}</router-link></li>
	</ul>
</template>

<script>
	export default{
		name:"",
		data(){/* 数据存放 */
			return{
				navData:[
					{name:"喜剧",to:"/xiju",buer:true},
					{name:"体育",to:"/tiyu",buer:false},
					{name:"亲子",to:"/qinzi",buer:false},
					{name:"舞蹈古典",to:"/wudaogudian",buer:false},
					{name:"摇滚",to:"/yaogun",buer:false}
				]
			}
		},
		mounted() {  /* 开始时自动执行*/
			
		},
		methods:{  /* 方法区*/
			
		},
		components:{/* 组件区 */
			
		},
	}
</script>

<style scoped="scoped">
	.header-shouye{
		padding: 0;
	}
	.header-shouye ul li{
		width: 100px;
		height: 64px;
		list-style: none;
		display: inline-block;
		color: #000;
		font-size: 18px;
		text-align: center;
	}
	.header-shouye .active{
		color: #FFFFFF;
		background-color: #FF3C1B;
	}
	.header-shouye a{
		width: 100px;
		height: 64px;
		color: #000000;
		display: block;
	}
</style>
