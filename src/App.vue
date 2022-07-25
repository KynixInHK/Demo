<script setup>
  const choose = (e) => {
    // console.log(e)
    const td = document.getElementById(e.target.dataset.id)
    // console.log(td)
    td.style.backgroundColor = 'blue'
  }
</script>

<template>
    <table border="1">
        <tr>
            <td id="1"></td>
            <td id="2"></td>
            <td id="3"></td>
            <td id="4"></td>
            <td id="5"></td>
        </tr>
    </table>
    <form action="#">
              <view class="questions">
            <view>1.</view>
            <input type="radio" name="yesorno1" data-id="1" value="yes" @click="choose">是
            <input type="radio" name="yesorno1" data-id="1" value="no" @click="choose">否
        </view>

        <view class="questions">
            <view>2.</view>
            <input type="radio" name="yesorno2" data-id="2" value="yes" @click="choose">是
            <input type="radio" name="yesorno2" data-id="2" value="no" @click="choose">否
        </view>

        <view class="questions">
            <view>3.</view>
            <input type="radio" name="yesorno3" data-id="3" value="yes" @click="choose">是
            <input type="radio" name="yesorno3" data-id="3" value="no" @click="choose">否
        </view>

        <view class="questions">
            <view>4.</view>
            <input type="radio" name="yesorno4" data-id="4" value="yes" @click="choose">是
            <input type="radio" name="yesorno4" data-id="4" value="no" @click="choose">否
        </view>

        <view class="questions">
            <view>5.</view>
            <input type="radio" name="yesorno5" data-id="5" value="yes" @click="choose">是
            <input type="radio" name="yesorno5" data-id="5" value="no" @click="choose">否
        </view>

    </form>
</template>

<style scoped>
  td {
    width: 50px;
    height: 20px;
  }
  .questions {
    display: block;
  }
</style>
