#### FLEX


[ISUX -> 移动端全兼容的flexbox速成班](https://isux.tencent.com/flexbox.html)

## exampel

	<div class="flex-box">
		<div class="flex-item">1</div>
		<div class="flex-item">2</div>
		<div class="flex-item">3</div>
		<div class="flex-item">1.1</div>
		<div class="flex-item">2.1</div>
		<div class="flex-item">3.1</div>
		<div class="flex-item">1.2</div>
		<div class="flex-item">2.2</div>
		<div class="flex-item">3.2</div>
	</div>
	<style>
		.flex-box{
			display: flex;
			width: 500px;
			height: 300px;
			/*flex-direction 指定元素以何种方式排列 row row-reverse column column-reverse*/
			/*row -> 列 column -> 行*/
			/*flex-direction: row;*/
			/*换行 和元素flex值关联 wrap-reverse -> 也是换行，表现形式不一样*/
			flex-wrap: wrap;
			/*定义父容器内元素水平方向的空间*/
			justify-content: flex-end;
			/*定义父容器内元素垂直方向的空间*/
			/*align-content: space-between;*/
			/*定义父容器内元素垂直方向的对齐方式*/
			/*align-items: center;*/
		}
		.flex-box > div{
			flex: auto;
			background: #ccc;
		}
		.flex-item:first-child{
			width: 500px;
			background: #956;
			/*定义item拉伸值 不能为负值*/
			/*flex-grow: 10;*/
			/*定义item收缩值 不能为负值*/
			/*flex-shrink: 2;*/
			/*定义排序优先值*/
			order: 2;
		}
		.flex-item:nth-child(2n){
			background: #965;
			/*定义item拉伸值 不能为负值*/
			flex-grow: 2;
			/*定义排序优先值*/
			order: 1;
		}
		.flex-item:nth-child(3n){
			background: #556;
			/*定义item拉伸值 不能为负值*/
			flex-grow: 3;
			/*定义排序优先值*/
			order: 3;
		}
	</style>