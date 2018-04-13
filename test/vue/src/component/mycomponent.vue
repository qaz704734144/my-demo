<<template >
 <div id='example-3'>
  <input type="checkbox" id="jack" value="Jack" v-model="checkedNames">
  <label for="jack">Jack</label>
  <input type="checkbox" id="john" value="John" v-model="checkedNames">
  <label for="john">John</label>
  <input type="checkbox" id="mike" value="Mike" v-model="checkedNames">
  <label for="mike">Mike</label>
  <br>
  <span>Checked names: {{ checkedNames }}</span>
  <br>
  <br>
  <br>
  <input type="text" v-model="messages">
<p>这是输入框的值：{{messages}}</p>
<br>
<br>
<ul id="example-1">
  <li v-for="(item,key,index) in items">
    {{index}}-{{key}}-{{ item }}
  </li>
</ul>
</div>

</template>

<script>
export default {
    data () {
    return {
        checkedNames: [],
        messages:"",
        items: {
            firstName: 'John',
            lastName: 'Doe',
            age: 30,
            addr:"广州市白云区中海金沙湾",
            gender:"boy"
          }
    }
  }
}
</script>

<style>

</style>