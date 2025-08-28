<template>
  <div >

    <el-row  style=" margin-top:5px; margin-left:15px; margin-right:15px;">
      <el-col :span="2" style="min-height:1px;">
        <div></div>
      </el-col>
      <el-col :span="4" >
        <div class="progress-box">
          <el-button type="text" style="margin-right:5px;" >电机01最大电流</el-button>
          <el-input v-model="dataInput.Data1Input" style="width: 100%;" size="mini" readonly/>
          <InputHex :inputs.sync="dataInput.Addr1Input" style="width: 100%;" size="mini" ></InputHex>
        </div>
      </el-col>
      <el-col :span="4" >
        <div class="progress-box">
          <el-button type="text" style="margin-right:5px;">电机02最大电流:</el-button>
          <el-input v-model="dataInput.Data1Input" style="width: 100%;" size="mini" readonly/>
          <InputHex :inputs.sync="dataInput.Addr1Input" style="width: 100%;" size="mini" ></InputHex>
        </div>
      </el-col>
      <el-col :span="4" >
        <div class="progress-box">
          <el-button type="text" style="margin-right:5px;" >电机03最大电流:</el-button>
          <el-input v-model="dataInput.Data1Input" style="width: 100%;" size="mini" readonly/>
          <InputHex :inputs.sync="dataInput.Addr1Input" style="width: 100%;" size="mini" ></InputHex>
        </div>
      </el-col>  
      <el-col :span="4" >
        <div class="progress-box">
          <el-button type="text" style="margin-right:5px;" >电机04最大电流:</el-button>
          <el-input v-model="dataInput.Data1Input" style="width: 100%;" size="mini" readonly/>
          <InputHex :inputs.sync="dataInput.Addr1Input" style="width: 100%;" size="mini" ></InputHex>
        </div>
      </el-col>  
      <el-col :span="4" >
        <div class="progress-box">
          <el-button type="text" style="margin-right:5px;" >电机05最大电流:</el-button>
          <el-input v-model="dataInput.Data1Input" style="width: 100%;" size="mini" readonly/>
          <InputHex :inputs.sync="dataInput.Addr1Input" style="width: 100%;" size="mini" ></InputHex>
        </div>
      </el-col> 
      <el-col :span="2" style="min-height:1px;">
        <div></div>
      </el-col>
    </el-row>   


  <el-row  style="margin-top:5px; margin-left:15px; margin-right:15px;">
     <el-col :span="2" style="min-height:1px;">
        <div></div>
      </el-col>
      <el-col :span="4" >
        <div class="progress-box">
          <el-button type="text" style="margin-right:5px;" >电机06最大电流:</el-button>
          <el-input v-model="dataInput.Data1Input" style="width: 100%;" size="mini" readonly/>
          <InputHex :inputs.sync="dataInput.Addr1Input" style="width: 100%;" size="mini" ></InputHex>
        </div>
      </el-col>
      <el-col :span="4" >
        <div class="progress-box">
          <el-button type="text" style="margin-right:5px;">电机07最大电流:</el-button>
          <el-input v-model="dataInput.Data1Input" style="width: 100%;" size="mini" readonly/>
          <InputHex :inputs.sync="dataInput.Addr1Input" style="width: 100%;" size="mini" ></InputHex>
        </div>
      </el-col>
      <el-col :span="4" >
        <div class="progress-box">
          <el-button type="text" style="margin-right:5px;">电机08最大电流:</el-button>
          <el-input v-model="dataInput.Data1Input" style="width: 100%;" size="mini" readonly/>
          <InputHex :inputs.sync="dataInput.Addr1Input" style="width: 100%;" size="mini" ></InputHex>
        </div>
      </el-col>  
      <el-col :span="4" >
        <div class="progress-box">
          <el-button type="text" style="margin-right:5px;">电机09最大电流:</el-button>
          <el-input v-model="dataInput.Data1Input" style="width: 100%;" size="mini" readonly/>
          <InputHex :inputs.sync="dataInput.Addr1Input" style="width: 100%;" size="mini" ></InputHex>
        </div>
      </el-col>  
      <el-col :span="4" >
        <div class="progress-box">
          <el-button type="text" style="margin-right:5px;">电机10最大电流:</el-button>
          <el-input v-model="dataInput.Data1Input" style="width: 100%;" size="mini" readonly/>
          <InputHex :inputs.sync="dataInput.Addr1Input" style="width: 100%;" size="mini" ></InputHex>
        </div>
      </el-col> 
      <el-col :span="2" style="min-height:1px;">
        <div></div>
      </el-col>
  </el-row>   

  <el-row  style="margin-top:5px; margin-left:15px; margin-right:15px;">
     <el-col :span="2" style="min-height:1px;">
        <div></div>
      </el-col>
      <el-col :span="4" >
        <div class="progress-box">
          <el-button type="text" style="margin-right:5px;" >电机11最大电流:</el-button>
          <el-input v-model="dataInput.Data1Input" style="width: 100%;" size="mini" readonly/>
          <InputHex :inputs.sync="dataInput.Addr1Input" style="width: 100%;" size="mini" ></InputHex>
        </div>
      </el-col>
      <el-col :span="4" >
        <div class="progress-box">
          <el-button type="text" style="margin-right:5px;" >电机12最大电流:</el-button>
          <el-input v-model="dataInput.Data1Input" style="width: 100%;" size="mini" readonly/>
          <InputHex :inputs.sync="dataInput.Addr1Input" style="width: 100%;" size="mini" ></InputHex>
        </div>
      </el-col>
      <el-col :span="4" >
        <div class="progress-box">
          <el-button type="text" style="margin-right:5px;" >电机13最大电流:</el-button>
          <el-input v-model="dataInput.Data1Input" style="width: 100%;" size="mini" readonly/>
          <InputHex :inputs.sync="dataInput.Addr1Input" style="width: 100%;" size="mini" ></InputHex>
        </div>
      </el-col>  
      <el-col :span="4" >
        <div class="progress-box">
          <el-button type="text" style="margin-right:5px;" >电机14最大电流:</el-button>
          <el-input v-model="dataInput.Data1Input" style="width: 100%;" size="mini" readonly/>
          <InputHex :inputs.sync="dataInput.Addr1Input" style="width: 100%;" size="mini" ></InputHex>
        </div>
      </el-col>  
      <el-col :span="4" >
        <div class="progress-box">
          <el-button type="text" style="margin-right:5px;" >电机15最大电流:</el-button>
          <el-input v-model="dataInput.Data1Input" style="width: 100%;" size="mini" readonly/>
          <InputHex :inputs.sync="dataInput.Addr1Input" style="width: 100%;" size="mini" ></InputHex>
        </div>
      </el-col> 
      <el-col :span="2" style="min-height:1px;">
        <div></div>
      </el-col>
  </el-row>   

  
  <el-row  style="margin-top:5px; margin-left:15px; margin-right:15px;">
     <el-col :span="6" style="min-height:1px;">
        <div></div>
      </el-col>
      <el-col :span="8" >
        <el-button size="mini" @click="saveRadio3">读取电机最大电流</el-button>
      </el-col>
      <el-col :span="8" >
        <el-button size="mini" @click="saveRadio3">写入电机最大电流</el-button>
      </el-col> 
      <el-col :span="6" style="min-height:1px;">
        <div></div>
      </el-col>
  </el-row>   
</div>    
</template>

<script>
import InputNumber from '@/components/InputNumber'
import InputHex from '@/components/InputHex'
import { ipcRenderer } from 'electron'
import {
  APP_WATCH_DATA_REFRESH,
  APP_WATCH_DATA,
} from '../../../../js/constants/IndoorConstants'
export default {
data () {
  return {
    dataInput: {
      Addr1Input : '0',
      Addr2Input : '0',
      Addr3Input : '0',
      Addr4Input : '0',
      Addr5Input : '0',
      Data1Input : '',
      Data2Input : '',
      Data3Input : '',
      Data4Input : '',
      Data5Input : '',
    },
    isClick:false
  }
},

components: {
  InputNumber,
  InputHex
},

beforeCreate: function () {
  this.$store.dispatch('CleanFilelist') 
},

created: function () {
  ipcRenderer.on(APP_WATCH_DATA_REFRESH, (event, arg) => {
    
      this.dataInput.Data1Input = arg[0] << 8 | arg[1]    //数据1
      this.dataInput.Data2Input = arg[2] << 8 | arg[3]    //数据2
      this.dataInput.Data3Input = arg[4] << 8 | arg[5]    //数据3
      // this.dataInput.Data4Input = arg[6] << 8 | arg[7]    //数据4
      // this.dataInput.Data5Input = arg[8] << 8 | arg[9]    //数据5
    
  })
},
watch: {
    ['dataInput.Addr1Input'](value) {
        if (value.toString().length === 4) {
            let data = []
            data[0]  = this.dataInput.Addr1Input
            data[1]  = this.dataInput.Addr2Input
            data[2]  = this.dataInput.Addr3Input
            data[3]  = this.dataInput.Addr4Input
            data[4]  = this.dataInput.Addr5Input
            ipcRenderer.send(APP_WATCH_DATA, 
            {
              addr: data,
            })
        } 
    },
    ['dataInput.Addr2Input'](value) {
        if (value.toString().length === 4) {
            let data = []
            data[0]  = this.dataInput.Addr1Input
            data[1]  = this.dataInput.Addr2Input
            data[2]  = this.dataInput.Addr3Input
            data[3]  = this.dataInput.Addr4Input
            data[4]  = this.dataInput.Addr5Input
            ipcRenderer.send(APP_WATCH_DATA,
            {
              addr: data,
            })
        } 
    },
    ['dataInput.Addr3Input'](value) {
      if (value.toString().length === 4) {
          let data = []
          data[0]  = this.dataInput.Addr1Input
          data[1]  = this.dataInput.Addr2Input
          data[2]  = this.dataInput.Addr3Input
          data[3]  = this.dataInput.Addr4Input
          data[4]  = this.dataInput.Addr5Input
          ipcRenderer.send(APP_WATCH_DATA, 
          {
            addr: data,
          })
      }
    },
    ['dataInput.Addr4Input'](value) {
      if (value.toString().length === 4) {
          let data = []
          data[0]  = this.dataInput.Addr1Input
          data[1]  = this.dataInput.Addr2Input
          data[2]  = this.dataInput.Addr3Input
          data[3]  = this.dataInput.Addr4Input
          data[4]  = this.dataInput.Addr5Input
          ipcRenderer.send(APP_WATCH_DATA, 
          {
            addr: data,
          })
      } 
  },
  ['dataInput.Addr5Input'](value) {
    if (value.toString().length === 4) {
        let data = []
        data[0]  = this.dataInput.Addr1Input
        data[1]  = this.dataInput.Addr2Input
        data[2]  = this.dataInput.Addr3Input
        data[3]  = this.dataInput.Addr4Input
        data[4]  = this.dataInput.Addr5Input
        ipcRenderer.send(APP_WATCH_DATA,
        {
          addr: data,
        })
    }
  },
  }
}
</script>

<style scoped>
.progress-box {
  display: flex;
  align-items: center;
}
.el-col-4{
  margin-left: 8px;
}
</style>
