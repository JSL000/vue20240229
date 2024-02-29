<script>
export default {
    data() {
    },
};
</script>

<template>
    <div class="w-screen mt-2">
        <div class="bg-gray-100 p-6 rounded-xl shadow-md">
            <h1 class="text-3xl font-bold mb-5 text-black">To-Do List</h1>
            <div class="flex mb-4">
                <input class="border border-gray-300 text-black rounded-l-md px-3 py-2 w-full">
                <button @click="addTodo" class="bg-blue-500 text-black px-4 py-2 rounded-r-md">新增</button>
            </div>
            <div class="flex mb-4">
                <button class="bg-blue-500 text-white px-4 py-2 rounded-l-md">新增</button>
                <button class="bg-blue-500 text-white px-4 py-2">已執行</button>
                <button class="bg-blue-500 text-white px-4 py-2 rounded-r-md">未執行</button>
            </div>
            <table class="w-5/6 text-black">
                <thead>
                    <tr>
                        <th>執行</th>
                        <th>事項</th>
                        <th>功能</th>
                    </tr>
                </thead>

                <tbody class="data-show">

                </tbody>
            </table>
            <hr class="bg-slate-950 h-0.5">
            <ul>
                <li class="flex items-center justify-between text-black py-2">
                    <div class="flex items-center">
                        <input type="checkbox" class="mr-20">
                        <span>第一筆</span>
                    </div>
                    <div>
                        <button class="text-blue-500 mr-2">編輯</button>
                        <button class="text-red-500 mr-2">刪除</button>
                    </div>
                </li>
            </ul>
            <button class="bg-gray-300 text-gray-600 px-4 py-2 rounded-r-md">存入local</button>
        </div>
    </div>
</template>

<style scoped></style>