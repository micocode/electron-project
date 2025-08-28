<template>
  <div class="out-table">
    <div class="block">
      <el-carousel
        height="150px"
        indicator-position="outside"
        :autoplay="false"
      >
        <el-carousel-item>
          <el-radio-group v-model="radio1" style="margin-top:5px">
            <el-row type="flex" justify="center">
              <el-col :span="2" >
                <div></div>
              </el-col>
              <el-col :span="4">
                <el-radio :label="1">编码器01零点偏置&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="4">
                <el-radio :label="2">编码器02零点偏置&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="4">
                <el-radio :label="3">编码器03零点偏置&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="4">
                <el-radio :label="4">编码器04零点偏置&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="4">
                <el-radio :label="5">编码器05零点偏置&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="2" >
                <div></div>
              </el-col>
            </el-row>
            <el-row type="flex" justify="center">
              <el-col :span="2" >
                <div></div>
              </el-col>
              <el-col :span="4">
                <el-radio :label="6">编码器06零点偏置&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="4">
                <el-radio :label="7">编码器07零点偏置&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="4">
                <el-radio :label="8">编码器08零点偏置&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="4">
                <el-radio :label="9">编码器09零点偏置&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="4">
                <el-radio :label="10">编码器10零点偏置&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="2">
                <div></div>
              </el-col>
            </el-row>
            <el-row type="flex" justify="center">
              <el-col :span="2">
                <div></div>
              </el-col>
              <el-col :span="4">
                <el-radio :label="11">编码器11零点偏置&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="4">
                <el-radio :label="12">编码器12零点偏置&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="4">
                <el-radio :label="13">编码器13零点偏置&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="4">
                <el-radio :label="14">编码器14零点偏置&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="4">
                <el-radio :label="15">编码器15零点偏置&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="2">
                <div></div>
              </el-col>
            </el-row>
            <el-row type="flex" justify="center">
              <el-col :span="3" style="min-height:1px;">
                <div></div>
              </el-col>
              <el-col :span="16">
                <div class="table-input">
                  <el-button type="text" size="mini">更改数据值：</el-button>
                  <el-input placeholder="请输入数据" v-model="DataType.Data"></el-input>
                </div>
              </el-col>
              <el-col :span="3">
                <el-button size="mini" @click="saveRadio1">确认修改</el-button>
              </el-col>
              <el-col :span="2" style="min-height:1px;">
                <div></div>
              </el-col>
            </el-row>
          </el-radio-group>
        </el-carousel-item>
        <el-carousel-item>
          <el-radio-group v-model="radio2" style="margin-top:10px">
            <el-row type="flex" justify="center">
              <el-col :span="2" >
                <div></div>
              </el-col>
              <el-col :span="4">
                <el-radio :label="1">编码器01顺逆方向&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="4">
                <el-radio :label="2">编码器02顺逆方向&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="4">
                <el-radio :label="3">编码器03顺逆方向&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="4">
                <el-radio :label="4">编码器04顺逆方向&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="4">
                <el-radio :label="5">编码器05顺逆方向&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="2" >
                <div></div>
              </el-col>
            </el-row>
            <el-row type="flex" justify="center">
              <el-col :span="2" >
                <div></div>
              </el-col>
              <el-col :span="4">
                <el-radio :label="6">编码器06顺逆方向&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="4">
                <el-radio :label="7">编码器07顺逆方向&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="4">
                <el-radio :label="8">编码器08顺逆方向&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="4">
                <el-radio :label="9">编码器09顺逆方向&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="4">
                <el-radio :label="10">编码器10顺逆方向&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="2">
                <div></div>
              </el-col>
            </el-row>
            <el-row type="flex" justify="center">
              <el-col :span="2">
                <div></div>
              </el-col>
              <el-col :span="4">
                <el-radio :label="11">编码器11顺逆方向&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="4">
                <el-radio :label="12">编码器12顺逆方向&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="4">
                <el-radio :label="13">编码器13顺逆方向&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="4">
                <el-radio :label="14">编码器14顺逆方向&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="4">
                <el-radio :label="15">编码器15顺逆方向&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="2">
                <div></div>
              </el-col>
            </el-row>
            <el-row type="flex" justify="center">
              <el-col :span="2" style="min-height:1px;">
                <div></div>
              </el-col>
              <el-col :span="17">
                <div class="table-input">
                  <el-button type="text" size="mini">更改数据值：</el-button>
                  <el-input placeholder="0:顺时针, 1:逆时针" v-model="DataType.Data"></el-input>
                </div>
              </el-col>
              <el-col :span="3">
                <el-button size="mini" @click="saveRadio2">确认修改</el-button>
              </el-col>
              <el-col :span="2" style="min-height:1px;">
                <div></div>
              </el-col>
            </el-row>
          </el-radio-group>
        </el-carousel-item>
        <el-carousel-item>
          <el-radio-group v-model="radio3" style="margin-top:10px">
             <el-row type="flex" justify="center">
              <el-col :span="2" >
                <div></div>
              </el-col>
              <el-col :span="4">
                <el-radio :label="1">关节和电机01映射关系&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="4">
                <el-radio :label="2">关节和电机02映射关系&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="4">
                <el-radio :label="3">关节和电机03映射关系&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="4">
                <el-radio :label="4">关节和电机04映射关系&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="4">
                <el-radio :label="5">关节和电机05映射关系&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="2" >
                <div></div>
              </el-col>
            </el-row>
            <el-row type="flex" justify="center">
              <el-col :span="2" >
                <div></div>
              </el-col>
              <el-col :span="4">
                <el-radio :label="6">关节和电机06映射关系&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="4">
                <el-radio :label="7">关节和电机07映射关系&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="4">
                <el-radio :label="8">关节和电机08映射关系&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="4">
                <el-radio :label="9">关节和电机09映射关系&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="4">
                <el-radio :label="10">关节和电机10映射关系&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="2">
                <div></div>
              </el-col>
            </el-row>
            <el-row type="flex" justify="center">
              <el-col :span="2">
                <div></div>
              </el-col>
              <el-col :span="4">
                <el-radio :label="11">关节和电机11映射关系&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="4">
                <el-radio :label="12">关节和电机12映射关系&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="4">
                <el-radio :label="13">关节和电机13映射关系&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="4">
                <el-radio :label="14">关节和电机14映射关系&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="4">
                <el-radio :label="15">关节和电机15映射关系&ensp;&ensp;</el-radio>
              </el-col>
              <el-col :span="2">
                <div></div>
              </el-col>
            </el-row>
            <el-row type="flex" justify="center">
              <el-col :span="2" style="min-height:1px;">
                <div></div>
              </el-col>
              <el-col :span="17 ">
                <div class="table-input">
                  <el-button type="text" size="mini">更改数据值：</el-button>
                  <el-input placeholder="0:手指弯曲关节增大, 1:手指弯曲关节减少" v-model="DataType.Data"></el-input>
                </div>
              </el-col>
              <el-col :span="3">
                <el-button size="mini" @click="saveRadio3">确认修改</el-button>
              </el-col>
              <el-col :span="2" style="min-height:1px;">
                <div></div>
              </el-col>
            </el-row>
          </el-radio-group>
        </el-carousel-item>
      </el-carousel>
    </div>
  </div>
</template>

<script>
  import { ipcRenderer } from 'electron'
  import {
    APP_TOUCH_BUTTON_SEND_MULT_CMD,
  } from '../../../../js/constants/IndoorConstants'
export default {
  name: "OutTable",
  data() {
    return {
      radio1: 1,
      radio2: 1,
      radio3: 1,
      DataInput: "",
      DataType: {
        Length: 1,
        Address: 0,
        Data: 0,
      }
    };
  },
  props: {
    tabItem: String
  },
  methods: {
    saveRadio1() {
      switch (this.radio1) {
        case 1:
          this.DataType.Address = 150;
          break;
        case 2:
          this.DataType.Address = 151;
          break;
        case 3:
          this.DataType.Address = 152;
          break;
        case 4:
          this.DataType.Address = 153;
          break;
        case 5:
          this.DataType.Address = 154;
          break;
        case 6:
          this.DataType.Address = 155;
          break;
        case 7:
          this.DataType.Address = 156;
          break;
        case 8:
          this.DataType.Address = 157;
          break;
        case 9:
          this.DataType.Address = 158;
          break;
        case 10:
          this.DataType.Address = 159;
          break;
        default:
          break;
      }
      ipcRenderer.send(APP_TOUCH_BUTTON_SEND_MULT_CMD, {
        Length: this.DataType.Length,
        Address: this.DataType.Address,
        Data: this.DataType.Data,

      })
      //console.log("radio1>>", this.radio1);
    },
    saveRadio2() {
       switch (this.radio2) {
        case 1:
          this.DataType.Address = 160;
          break;
        case 2:
          this.DataType.Address = 161;
          break;
        case 3:
          this.DataType.Address = 162;
          break;
        case 4:
          this.DataType.Address = 163;
          break;
        case 5:
          this.DataType.Address = 164;
          break;
        case 6:
          this.DataType.Address = 165;
          break;
        case 7:
          this.DataType.Address = 166;
          break;
        case 8:
          this.DataType.Address = 167;
          break;
        case 9:
          this.DataType.Address = 168;
          break;
        case 10:
          this.DataType.Address = 169;
          break;
        default:
          break;
      }
      ipcRenderer.send(APP_TOUCH_BUTTON_SEND_MULT_CMD, {
        Length: this.DataType.Length,
        Address: this.DataType.Address,
        Data: this.DataType.Data,

      })
      //console.log("radio2>>", this.radio2);
    },
    saveRadio3() {
       switch (this.radio3) {
        case 1:
          this.DataType.Address = 170;
          break;
        case 2:
          this.DataType.Address = 171;
          break;
        case 3:
          this.DataType.Address = 172;
          break;
        case 4:
          this.DataType.Address = 173;
          break;
        case 5:
          this.DataType.Address = 174;
          break;
        case 6:
          this.DataType.Address = 175;
          break;
        case 7:
          this.DataType.Address = 176;
          break;
        case 8:
          this.DataType.Address = 177;
          break;
        case 9:
          this.DataType.Address = 178;
          break;
        case 10:
          this.DataType.Address = 179;
          break;
        default:
          break;
      }
      ipcRenderer.send(APP_TOUCH_BUTTON_SEND_MULT_CMD, {
        Length: this.DataType.Length,
        Address: this.DataType.Address,
        Data: this.DataType.Data,

      })
      //console.log("radio3>>", this.radio3);
    },
    saveRadio4() {
       switch (this.radio4) {
        case 1:
          this.DataType.Address = 180;
          break;
        case 2:
          this.DataType.Address = 181;
          break;
        case 3:
          this.DataType.Address = 182;
          break;
        case 4:
          this.DataType.Address = 183;
          break;
        case 5:
          this.DataType.Address = 184;
          break;
        case 6:
          this.DataType.Address = 185;
          break;
        case 7:
          this.DataType.Address = 186;
          break;
        case 8:
          this.DataType.Address = 187;
          break;
        case 9:
          this.DataType.Address = 188;
          break;
        case 10:
          this.DataType.Address = 189;
          break;
        default:
          break;
      }
      ipcRenderer.send(APP_TOUCH_BUTTON_SEND_MULT_CMD, {
        Length: this.DataType.Length,
        Address: this.DataType.Address,
        Data: this.DataType.Data,

      })
      //console.log("radio4>>", this.radio5);
    },
    saveRadio5() {
       switch (this.radio5) {
        case 1:
          this.DataType.Address = 190;
          break;
        case 2:
          this.DataType.Address = 191;
          break;
        case 3:
          this.DataType.Address = 192;
          break;
        case 4:
          this.DataType.Address = 193;
          break;
        case 5:
          this.DataType.Address = 194;
          break;
        case 6:
          this.DataType.Address = 195;
          break;
        case 7:
          this.DataType.Address = 243;
          break;
        case 8:
          this.DataType.Address = 244;
          break;
        case 9:
          this.DataType.Address = 245;
          break;
        case 10:
          this.DataType.Address = 246;
          break;
        default:
          break;
      }
      ipcRenderer.send(APP_TOUCH_BUTTON_SEND_MULT_CMD, {
        Length: this.DataType.Length,
        Address: this.DataType.Address,
        Data: this.DataType.Data,

      })
      //console.log("radio5>>", this.radio5);
    },
    saveRadio6() {
       switch (this.radio6) {
        case 1:
          this.DataType.Address = 214;
          break;
        case 2:
          this.DataType.Address = 215;
          break;
        case 3:
          this.DataType.Address = 216;
          break;
        case 4:
          this.DataType.Address = 217;
          break;
        case 5:
          this.DataType.Address = 218;
          break;
        case 6:
          this.DataType.Address = 219;
          break;
        case 7:
          this.DataType.Address = 220;
          break;
        case 8:
          this.DataType.Address = 221;
          break;
        case 9:
          this.DataType.Address = 222;
          break;
        case 10:
          this.DataType.Address = 223;
          break;
        default:
          break;
      }
      ipcRenderer.send(APP_TOUCH_BUTTON_SEND_MULT_CMD, {
        Length: this.DataType.Length,
        Address: this.DataType.Address,
        Data: this.DataType.Data,

      })
      //console.log("radio6>>", this.radio6);
    },
    saveRadio7() {
       switch (this.radio7) {
        case 1:
          this.DataType.Address = 224;
          break;
        case 2:
          this.DataType.Address = 225;
          break;
        case 3:
          this.DataType.Address = 226;
          break;
        case 4:
          this.DataType.Address = 227;
          break;
        case 5:
          this.DataType.Address = 228;
          break;
        case 6:
          this.DataType.Address = 229;
          break;
        case 7:
          this.DataType.Address = 230;
          break;
        case 8:
          this.DataType.Address = 231;
          break;
        case 9:
          this.DataType.Address = 232;
          break;
        case 10:
          this.DataType.Address = 233;
          break;
        default:
          break;
      }
      ipcRenderer.send(APP_TOUCH_BUTTON_SEND_MULT_CMD, {
        Length: this.DataType.Length,
        Address: this.DataType.Address,
        Data: this.DataType.Data,

      })
      //console.log("radio7>>", this.radio7);
    },
    saveRadio8() {
       switch (this.radio8) {
        case 1:
          this.DataType.Address = 252;
          break;
        case 2:
          this.DataType.Address = 241;
          break;
        case 3:
          this.DataType.Address = 242;
          break;
        case 4:
          this.DataType.Address = 207;
          break;
        case 5:
          this.DataType.Address = 249;
          break;
        case 6:
          this.DataType.Address = 247;
          break;
        case 7:
          this.DataType.Address = 211;
          break;
        case 8:
          this.DataType.Address = 212;
          break;
        case 9:
          this.DataType.Address = 248;
          break;
        case 10:
          this.DataType.Address = 251;
          break;
        default:
          break;
      }
      ipcRenderer.send(APP_TOUCH_BUTTON_SEND_MULT_CMD, {
        Length: this.DataType.Length,
        Address: this.DataType.Address,
        Data: this.DataType.Data,

      })
      //console.log("radio8>>", this.radio8);
    }
  },
  computed:{
    isShow(){
      return this.tabItem==="8"?true:false
    }
  }
};
</script>

<style scoped>
.table-input {
  display: flex;
}
.el-row {
  margin-bottom: 20px;
}
.el-col {
  text-align: center;
}
</style>