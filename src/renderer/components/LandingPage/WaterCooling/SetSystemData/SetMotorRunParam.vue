<template>
    <div class="out-table">
      <div class="block">
        <el-carousel
          height="150px"
          indicator-position="outside"
          :autoplay="false"
        >
          <el-carousel-item>
            <el-checkbox-group v-model="checkList1" style="margin-top:2px">
              <el-row >
                <el-col :span="2" style="min-height:1px;" >
                  <div></div>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="1">设置电机01停止&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="2">设置电机02停止&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="3">设置电机03停止&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="4">设置电机04停止&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="5">设置电机05停止&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="2" style="min-height:1px;">
                  <div></div>
                </el-col>
              </el-row>
              <el-row>
                <el-col :span="2" style="min-height:1px;">
                  <div></div>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="6">设置电机06停止&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="7">设置电机07停止&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="8">设置电机08停止&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="9">设置电机09停止&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="10">设置电机10停止&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="2" style="min-height:1px;">
                  <div></div>
                </el-col>
              </el-row>
              <el-row>
                <el-col :span="2" style="min-height:1px;">
                  <div></div>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="11">设置电机11停止&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="12">设置电机12停止&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="13">设置电机13停止&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="14">设置电机14停止&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="15">设置电机15停止&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="2" style="min-height:1px;">
                  <div></div>
                </el-col>
              </el-row>
              <el-row type="flex" justify="center">
                <el-col :span="2" style="min-height:1px;">
                  <div></div>
                </el-col>
                <el-col :span="20">
                  <el-button size="mini" @click="saveCheckboxGroup1">发送电机关闭修改</el-button>
                </el-col>
                <el-col :span="2" style="min-height:1px;">
                  <div></div>
                </el-col>
              </el-row>
            </el-checkbox-group>
          </el-carousel-item>
        
          <el-carousel-item>
            <el-checkbox-group v-model="checkList2" style="margin-top:2px">
            <el-row >
                <el-col :span="2" style="min-height:1px;" >
                  <div></div>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="1">电机01重置零点&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="2">电机02重置零点&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="3">电机03重置零点&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="4">电机04重置零点&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="5">电机05重置零点&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="2" style="min-height:1px;">
                  <div></div>
                </el-col>
              </el-row>
              <el-row>
                <el-col :span="2" style="min-height:1px;">
                  <div></div>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="6">电机06重置零点&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="7">电机07重置零点&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="8">电机08重置零点&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="9">电机09重置零点&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="10">电机10重置零点&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="2" style="min-height:1px;">
                  <div></div>
                </el-col>
              </el-row>
              <el-row>
                <el-col :span="2" style="min-height:1px;">
                  <div></div>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="11">电机11重置零点&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="12">电机12重置零点&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="13">电机13重置零点&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="14">电机14重置零点&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="15">电机15重置零点&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="2" style="min-height:1px;">
                  <div></div>
                </el-col>
              </el-row>
              <el-row type="flex" justify="center">
                <el-col :span="2" style="min-height:1px;">
                  <div></div>
                </el-col>
                <el-col :span="20">
                  <el-button size="mini" @click="saveCheckboxGroup1">发送电机重置零点修改</el-button>
                </el-col>
                <el-col :span="2" style="min-height:1px;">
                  <div></div>
                </el-col>
              </el-row>
            </el-checkbox-group>
          </el-carousel-item>

          <el-carousel-item>
            <el-checkbox-group v-model="checkList3" style="margin-top:2px">
              <el-row >
                <el-col :span="2" style="min-height:1px;" >
                  <div></div>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="1">电机01转子零位校准&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="2">电机02转子零位校准&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="3">电机03转子零位校准&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="4">电机04转子零位校准&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="5">电机05转子零位校准&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="2" style="min-height:1px;">
                  <div></div>
                </el-col>
              </el-row>
              <el-row>
                <el-col :span="2" style="min-height:1px;">
                  <div></div>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="6">电机06转子零位校准&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="7">电机07转子零位校准&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="8">电机08转子零位校准&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="9">电机09转子零位校准&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="10">电机10转子零位校准&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="2" style="min-height:1px;">
                  <div></div>
                </el-col>
              </el-row>
              <el-row>
                <el-col :span="2" style="min-height:1px;">
                  <div></div>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="11">电机11转子零位校准&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="12">电机12转子零位校准&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="13">电机13转子零位校准&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="14">电机14转子零位校准&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="4">
                  <el-checkbox :label="15">电机15转子零位校准&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;</el-checkbox>
                </el-col>
                <el-col :span="2" style="min-height:1px;">
                  <div></div>
                </el-col>
              </el-row>
              <el-row type="flex" justify="center">
                <el-col :span="2" style="min-height:1px;">
                  <div></div>
                </el-col>
                <el-col :span="20">
                  <el-button size="mini" @click="saveCheckboxGroup1">发送电机转子零位校准修改</el-button>
                </el-col>
                <el-col :span="2" style="min-height:1px;">
                  <div></div>
                </el-col>
              </el-row>
            </el-checkbox-group>
          </el-carousel-item>
        </el-carousel>
      </div>
    </div>
  </template>
  
  <script>
    import { ipcRenderer } from 'electron'
    import {
      APP_SEND_SIGNAL_DATA_06_CMD
    } from '../../../../js/constants/IndoorConstants'
  export default {
    name: "OutTable",
    data() {
      return {
        checkList1: [],
        checkList2: [],
        checkList3: [],
        EEPROMType: {
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
      saveCheckboxGroup1(){
        console.log("checkList1>>", this.checkList1);
        this.EEPROMType.Data = 0;
        for (var i = 0; i < this.checkList1.length; i++) {
          switch(this.checkList1[i]) {
            case 1: 
              this.EEPROMType.Data |= 0x0001; 
              break;
            case 2:
              this.EEPROMType.Data |= 0x0002; 
              break;
            case 3:
              this.EEPROMType.Data |= 0x0004; 
              break;
            case 4:
              this.EEPROMType.Data |= 0x0008;  
              break;
            case 5:
              this.EEPROMType.Data |= 0x0010; 
              break;
            case 6:
              this.EEPROMType.Data |= 0x0020; 
              break;
            case 7:
              this.EEPROMType.Data |= 0x0040; 
              break;
            case 8:
              this.EEPROMType.Data |= 0x0080; 
              break;
            case 9:
              this.EEPROMType.Data |= 0x0100; 
              break;
            case 10:
              this.EEPROMType.Data |= 0x0200;  
              break;
            case 11:
              this.EEPROMType.Data |= 0x0400; 
              break;
            case 12:
              this.EEPROMType.Data |= 0x0800; 
              break;
            case 13:
              this.EEPROMType.Data |= 0x1000; 
              break;
            case 14:
              this.EEPROMType.Data |= 0x2000; 
              break;
            case 15:
              this.EEPROMType.Data |= 0x4000; 
              break;
            default:
                break;
          }
        }

        this.EEPROMType.Address = 234;
        ipcRenderer.send(APP_SEND_SIGNAL_DATA_06_CMD, {
          Length: this.EEPROMType.Length,
          Address: this.EEPROMType.Address,
          Data: this.EEPROMType.Data,
        })
           
      },
      saveCheckboxGroup2(){
        console.log("checkList2>>", this.checkList2);
        this.EEPROMType.Data = 0;
        for (var i = 0; i < this.checkList2.length; i++) {
          switch(this.checkList2[i]) {
            case 1: 
              this.EEPROMType.Data |= 0x0004; 
              break;
            case 2:
              this.EEPROMType.Data |= 0x0008; 
              break;
            case 3:
              this.EEPROMType.Data |= 0x0010; 
              break;
            case 4:
              this.EEPROMType.Data |= 0x0020; 
              break;
            case 5:
              this.EEPROMType.Data |= 0x0040; 
              break;
            case 6:
              this.EEPROMType.Data |= 0x0080; 
              break;
            case 7:
              this.EEPROMType.Data |= 0x0100; 
              break;
            case 8:
              this.EEPROMType.Data |= 0x0200; 
              break;
            case 9:
              this.EEPROMType.Data |= 0x0400; 
              break;
            case 10:
              this.EEPROMType.Data |= 0x0800; 
              break;
            case 11:
              this.EEPROMType.Data |= 0x1000; 
              break;
            case 12:
              this.EEPROMType.Data |= 0x2000; 
              break;
            case 13:
              this.EEPROMType.Data |= 0x4000; 
              break;
            case 14:
              this.EEPROMType.Data |= 0x8000; 
              break;
            default:
                break;
          }
        }

        this.EEPROMType.Address = 235;
        ipcRenderer.send(APP_SEND_SIGNAL_DATA_06_CMD, {
          Length: this.EEPROMType.Length,
          Address: this.EEPROMType.Address,
          Data: this.EEPROMType.Data,
        })
      },
      saveCheckboxGroup3(){
        console.log("checkList3>>", this.checkList3);
        this.EEPROMType.Data = 0;
        for (var i = 0; i < this.checkList3.length; i++) {
          switch(this.checkList3[i]) {
            case 1: 
              this.EEPROMType.Data |= 0x0001; 
              break;
            case 2:
              this.EEPROMType.Data |= 0x0002; 
              break;
            case 3:
              this.EEPROMType.Data |= 0x0004; 
              break;
            case 4:
              this.EEPROMType.Data |= 0x0008;  
              break;
            case 5:
              this.EEPROMType.Data |= 0x0010;  
              break;
            case 6:
              this.EEPROMType.Data |= 0x0020; 
              break;
            case 7:
              this.EEPROMType.Data |= 0x0040; 
              break;
            case 8:
              this.EEPROMType.Data |= 0x0080; 
              break;
            case 9:
              this.EEPROMType.Data |= 0x0100;  
              break;
            case 10:
              this.EEPROMType.Data |= 0x0200; 
              break;
            case 11:
              this.EEPROMType.Data |= 0x0400; 
              break;
            case 12:
              this.EEPROMType.Data |= 0x0800; 
              break;
            case 13:
              this.EEPROMType.Data |= 0x1000; 
              break;
            case 14:
              this.EEPROMType.Data |= 0x2000; 
              break;
            case 15:
              this.EEPROMType.Data |= 0x4000; 
              break;
            default:
                break;
          }
        }

        this.EEPROMType.Address = 236;
        ipcRenderer.send(APP_SEND_SIGNAL_DATA_06_CMD, {
          Length: this.EEPROMType.Length,
          Address: this.EEPROMType.Address,
          Data: this.EEPROMType.Data,
        })
      }, 
      saveCheckboxGroup4(){
        console.log("checkList4>>", this.checkList4);
        this.EEPROMType.Data = 0;
        for (var i = 0; i < this.checkList4.length; i++) {
          switch(this.checkList4[i]) {
            case 1: 
              this.EEPROMType.Data |= 0x0004; 
              break;
            case 2:
              this.EEPROMType.Data |= 0x0008; 
              break;
            case 3:
              this.EEPROMType.Data |= 0x0010; 
              break;
            case 4:
              this.EEPROMType.Data |= 0x0020; 
              break;
            case 5:
              this.EEPROMType.Data |= 0x0040; 
              break;
            case 6:
              this.EEPROMType.Data |= 0x0080; 
              break;
            case 7:
              this.EEPROMType.Data |= 0x0100; 
              break;
            case 8:
              this.EEPROMType.Data |= 0x0200; 
              break;
            case 9:
              this.EEPROMType.Data |= 0x0400; 
              break;
            case 10:
              this.EEPROMType.Data |= 0x0800; 
              break;
            case 11:
              this.EEPROMType.Data |= 0x1000; 
              break;
            case 12:
              this.EEPROMType.Data |= 0x2000; 
              break;
            case 13:
              this.EEPROMType.Data |= 0x4000; 
              break;
            case 14:
              this.EEPROMType.Data |= 0x8000; 
              break;
            default:
                break;
          }
        }

        this.EEPROMType.Address = 237;
        ipcRenderer.send(APP_SEND_SIGNAL_DATA_06_CMD, {
          Length: this.EEPROMType.Length,
          Address: this.EEPROMType.Address,
          Data: this.EEPROMType.Data,
        })
      },
      saveCheckboxGroup5(){
        console.log("checkList5>>", this.checkList5);

        this.EEPROMType.Data = 0;
        for (var i = 0; i < this.checkList5.length; i++) {
          switch(this.checkList5[i]) {
            case 1: 
              this.EEPROMType.Data |= 0x0001; // 水温高温告警 bit0
              break;
            case 2:
              this.EEPROMType.Data |= 0x0002; // 进水压力传感器故障 bit7
              break;
            case 3:
              this.EEPROMType.Data |= 0x0004; // 环境温度传感器故障  bit2
              break;
            case 4:
              this.EEPROMType.Data |= 0x0008; // 水泵压差低告警 bit9
              break;
            case 5:
              this.EEPROMType.Data |= 0x0010; // 出水温度传感器故障  bit4
              break;
            case 6:
              this.EEPROMType.Data |= 0x0020; // 水流开关保护告警 bit11
              break;
            case 7:
              this.EEPROMType.Data |= 0x0040; // 补水警告 bit10
              break;
            case 8:
              this.EEPROMType.Data |= 0x0080; // 水温低温告警 bit1
              break;
            case 9:
              this.EEPROMType.Data |= 0x0100; // 出水压力传感器故障 bit6
              break;
            case 10:
              this.EEPROMType.Data |= 0x0200; //系统水温传感器故障  bit3
              break;
             case 11:
              this.EEPROMType.Data |= 0x0400; //水泵压差高告警 bit8
              break;
            case 12:
              this.EEPROMType.Data |= 0x0800; //进水温度传感器故障 bit5
              break;
            case 13:
              this.EEPROMType.Data |= 0x1000; //水流开关保护锁定 bit12
              break;
            case 14:
              this.EEPROMType.Data |= 0x2000; // 温差过大告警 bit13
              break;
            case 15:
              this.EEPROMType.Data |= 0x4000; //水流开关保护锁定 bit12
              break;
            case 16:
              this.EEPROMType.Data |= 0x8000; // 温差过大告警 bit13
              break;
            default:
                break;
          }
        }

        this.EEPROMType.Address = 238;
        ipcRenderer.send(APP_SEND_SIGNAL_DATA_06_CMD, {
          Length: this.EEPROMType.Length,
          Address: this.EEPROMType.Address,
          Data: this.EEPROMType.Data,
        })
      },
      saveCheckboxGroup6(){
        console.log("checkList6>>", this.checkList6);
        this.EEPROMType.Data = 0;
        for (var i = 0; i < this.checkList6.length; i++) {
          switch(this.checkList6[i]) {
            case 1: 
              this.EEPROMType.Data |= 0x0001; 
              break;
            case 2:
              this.EEPROMType.Data |= 0x0002; 
              break;
            case 3:
              this.EEPROMType.Data |= 0x0004; 
              break;
            case 4:
              this.EEPROMType.Data |= 0x0008; 
              break;  
            case 5:
              this.EEPROMType.Data |= 0x0010; 
              break;
        
            default:
                break;
          }
        }

        this.EEPROMType.Address = 239;
        ipcRenderer.send(APP_SEND_SIGNAL_DATA_06_CMD, {
          Length: this.EEPROMType.Length,
          Address: this.EEPROMType.Address,
          Data: this.EEPROMType.Data,
        })
       
      },
      saveCheckboxGroup7(){
        console.log("checkList7>>", this.checkList7);
        this.EEPROMType.Data = 0;
        for (var i = 0; i < this.checkList7.length; i++) {
          switch(this.checkList7[i]) {
            case 1: 
              this.EEPROMType.Data |= 0x0001; 
              break;
            case 2:
              this.EEPROMType.Data |= 0x0002; 
              break;
            case 3:
              this.EEPROMType.Data |= 0x0004; 
              break;
            case 4:
              this.EEPROMType.Data |= 0x0008; 
              break;
            case 5:
              this.EEPROMType.Data |= 0x0010; 
              break;
            case 6:
              this.EEPROMType.Data |= 0x0020; 
              break;
            case 7:
              this.EEPROMType.Data |= 0x0040; 
              break;
            case 8:
              this.EEPROMType.Data |= 0x0080; 
              break;
            case 9:
              this.EEPROMType.Data |= 0x0100; 
              break;
            case 10:
              this.EEPROMType.Data |= 0x0200; 
              break;
            default:
                break;
          }
        }

        this.EEPROMType.Address = 240;
        ipcRenderer.send(APP_SEND_SIGNAL_DATA_06_CMD, {
          Length: this.EEPROMType.Length,
          Address: this.EEPROMType.Address,
          Data: this.EEPROMType.Data,
        }) 
      }

    },
    computed:{
      isShow(){
        return this.tabItem==="4"?true:false
      }
    }
  };
  </script>
  
  <style scoped>
  .table-input {
    display: flex;
  }
  .el-row {
    margin-bottom: 4px;
  }
  .el-col {
    text-align: center;
  }
  .el-col-5{
    margin-bottom: 4px;
  }
  .el-col-3{
    margin-bottom: 4px;
  }
  </style>