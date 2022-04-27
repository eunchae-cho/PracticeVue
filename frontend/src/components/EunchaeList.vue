<template>
    <div class="list">
        <div class="addBtn">
            <button class="btn btn-primary" @click="add()">+ 추가</button>
        </div>
        <ul>
            <li v-for="(c, idx) in content" :key="idx">{{ c }}</li>
        </ul>
    </div>
</template>

<script>
export default ({
    data() {
        const content = ['내용1', '내용2', '내용3', '내용4', '내용5'];
        const add = ()=> {
            content.push("추가 내용");
        }
        return {
            content,
            add
        }
    },
})
</script>


<style lang="scss" scoped>
.list ul {
    list-style: circle;

    li {
        padding : 15px;
        margin : 5px;
    }
}

.addBtn {
    text-align: right;

    button {
        margin : 12px;
    }
}
</style>