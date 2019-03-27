# Vue 组件的核心概念(VueComponentCoreConcept)：属性、事件、插槽

## Properties 属性

- 自定义属性 props: 组件 props 中声明的属性
- 原生属性 attrs: 没有生命的属性，默认自动挂载到组件根元素上，设置 inheritAttrs 为 false 可以关闭自动挂载
- 特殊属性 class | style: 挂载到组件根元素上，支持字符串、对象、数组等多种语法

## Event 事件

- 普通事件: @click @input @change @xxx 等事件，通过 this.$emit('xxx', ...) 触发
- 修饰符事件: @input.trim @click.stop @submit.prevent 等，一般用于原生 HTML 元素，自定义组件需要自行开发支持

## Slot 插槽

- 普通插槽: <template slot="xxx"></> <template v-slot:xxx></>
- 作用域插槽: <template slot="xxx" slot-scope="props"></> <template v-slot:xxx="props"></>

