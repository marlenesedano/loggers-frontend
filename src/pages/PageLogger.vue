<script setup lang="ts">
import Button from '../components/Button.vue';

</script>

<template>
    <div class="page">
        <div class="header">Loggers Sprint Boot</div>
        <div class="body">
            <div class="filter">
                <input type="text" class="filterInput"/>
                <Button description="Filtro/Total" class="buttonFilter"/>
            </div>
            <div class="tableData">
                <div>Root</div>
                <div>
                    <Button description="OFF"/>
                    <Button description="ERROR"/>
                    <Button description="WARN"/>
                    <Button description="INFO"/>
                    <Button description="DEBUG"/>
                    <Button description="TRACE"/>
                </div>
            </div>
        </div>
        <div class="footer"></div>
    </div>
</template>

<style scoped>
.page{
    /* background: #f5f5f5; */
}

.header {
    display: flex;
    justify-content: center;
    text-align: center;
    align-items: center;
    font-family: Inter, Avenir, Helvetica, Arial, sans-serif;
    font-size: 16px;
    line-height: 24px;
    font-weight: 400;
    background-color: blueviolet;
    height: 42px;
    color: white;
    margin-bottom: 22px;
}

.body {
    /* margin: 10px 100px; */
}

.filter {
    display: flex;
    align-items: center;
    justify-content: center;
}

.filterInput{
    width: 86%;
    padding: 6px 12px;
    border: 1px solid #dcdcdc;
    border-radius: 2px;
}

input::focus-visible {
    border: none;
}

.filterInput:focus {
    border: none;
}

.buttonFilter {
    padding: 6px 12px;
    border: 1px solid #dcdcdc;
}

.tableData {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    /* width: 70%; */
    align-items: center;
    text-align: center;
    padding: 8px 16px;
    margin: 20px 30px;
}


</style>
  