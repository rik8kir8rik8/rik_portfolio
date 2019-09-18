<template>
    <table id="skilltable">
      <td class="title-box">
        <div class="title">{{title}}</div>
        </td>
        <td class="text-sub">   
          <h2>{{subtitle}}</h2>
           <p>{{text}}</p>
        </td>
    </table>
</template>

<script>
export default {
  name: 'skilltable',
  props: {
      title:String,
      text:Object,
      subtitle:String
  }
}
</script>

<style lang="scss">
 @media screen and (min-width: 600px) {
      #skilltable{
        width:100%;
        height:15%;
          .title-box{
            display: table-cell;
                  text-align:center;
                  vertical-align: middle;
                  width:20%;
                  height:100%;
            .title{
                  display: table-cell;
                  height:50px;
                  width:50px;
                  text-align:center;
                  vertical-align: middle;
                  background:#616161;
                  color:#D3D5C6;
                  border-radius: 10px; 
                  font-size:50%;
                  border: 0.5px solid #000;
            }
          } 
          .text-sub{
          width: 70%;
                display: table-cell;
                  vertical-align: middle;
                  white-space:pre-wrap;
        }
      }
 }

  @media screen and (max-width: 600px) {
      #skilltable{
        width:100%;
        height:15%;
          .title-box{
            display: table-cell;
                  text-align:center;
                  vertical-align: middle;
                  width:30%;
                  height:100%;
            .title{
                  display: table-cell;
                  height:50px;
                  width:50px;
                  text-align:center;
                  vertical-align: middle;
                  background:#616161;
                  color:#D3D5C6;
                  border-radius: 10px; 
                  font-size:1.5rem;
                  border: 0.5px solid #000;
            }
          } 
          .text-sub{
          width: 70%;
                display: table-cell;
                  vertical-align: middle;
                  white-space:pre-wrap;
        }
      }
 }

 @media screen and (min-width: 600px) {
      #skilltable{
        width:100%;
        height:15%;
          .title-box{
            display: table-cell;
                  text-align:center;
                  vertical-align: middle;
                  width:30%;
                  height:100%;
            .title{
                  display: table-cell;
                  height:50px;
                  width:50px;
                  text-align:center;
                  vertical-align: middle;
                  background:#616161;
                  color:#D3D5C6;
                  border-radius: 10px; 
                  font-size:1.5rem;
                  border: 0.5px solid #000;
            }
          } 
          .text-sub{
          width: 70%;
                display: table-cell;
                  vertical-align: middle;
                  white-space: pre-wrap;
        }
      }
 }
</style>

