<template>
  <div >  
      <div >
        <fieldset style="background-color:#EBEEF5; borde-color: white;">
          <legend style="font:8px; font-weight:600;  margin-left:15px; margin-right:15px; margin-bottom:10px;">关节信息</legend> 
            <el-row  style=" margin-left:15px; margin-right:15px;">
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节01设定</el-button>
                  <el-input v-model="SystemData.SetJoint01" readonly size="mini"/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节02设定</el-button>
                  <el-input size="mini" v-model="SystemData.SetJoint02" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节03设定</el-button>
                  <el-input size="mini" v-bind:value="SystemData.SetJoint03" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节01位置</el-button>
                  <el-input size="mini" v-bind:value="SystemData.JointPos01" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节02位置</el-button>
                  <el-input size="mini" v-bind:value="SystemData.JointPos02" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节03位置</el-button>
                  <el-input size="mini" v-model="SystemData.JointPos03" readonly/>
                </div>
              </el-col>
            </el-row>

            <el-row  style=" margin-left:15px; margin-right:15px;">
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节04设定</el-button>
                  <el-input v-bind:value="SystemData.SetJoint04" readonly size="mini"/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节05设定</el-button>
                  <el-input size="mini" v-bind:value="SystemData.SetJoint05" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节06设定</el-button>
                  <el-input size="mini" v-bind:value="SystemData.SetJoint06" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节04位置</el-button>
                  <el-input size="mini" v-bind:value="SystemData.JointPos04" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节05位置</el-button>
                  <el-input size="mini" v-bind:value="SystemData.JointPos05" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节06位置</el-button>
                  <el-input size="mini" v-bind:value="SystemData.JointPos06 + KPaIcon" readonly/>
                </div>
              </el-col>
            </el-row>

            <el-row  style=" margin-left:15px; margin-right:15px;">
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节07设定</el-button>
                  <el-input v-bind:value="SystemData.SetJoint07" readonly size="mini"/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节08设定</el-button>
                  <el-input size="mini" v-bind:value="SystemData.SetJoint08" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节09设定</el-button>
                  <el-input size="mini" v-bind:value="SystemData.SetJoint09" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节07位置</el-button>
                  <el-input size="mini" v-bind:value="SystemData.JointPos07" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节08位置</el-button>
                  <el-input size="mini" v-bind:value="SystemData.JointPos08" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节09位置</el-button>
                  <el-input size="mini" v-model="SystemData.JointPos09" readonly/>
                </div>
              </el-col>
            </el-row>

            <el-row  style=" margin-left:15px; margin-right:15px;">
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节10设定</el-button>
                  <el-input size="mini" v-bind:value="SystemData.SetJoint10" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节11设定</el-button>
                  <el-input size="mini" v-bind:value="SystemData.SetJoint11" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节12设定</el-button>
                  <el-input size="mini" v-bind:value="SystemData.SetJoint12" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节10位置</el-button>
                  <el-input size="mini" v-bind:value="SystemData.JointPos10" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节11位置</el-button>
                  <el-input size="mini" v-bind:value="SystemData.JointPos11" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节12位置</el-button>
                  <el-input size="mini" v-bind:value="SystemData.JointPos12" readonly/>
                </div>
              </el-col>
            </el-row>

            <el-row  style=" margin-left:15px; margin-right:15px;">
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节13设定</el-button>
                  <el-input size="mini" v-bind:value="SystemData.SetJoint13" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节14设定</el-button>
                  <el-input size="mini" v-bind:value="SystemData.SetJoint14" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节15设定</el-button>
                  <el-input size="mini" v-bind:value="SystemData.SetJoint15" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节13位置</el-button>
                  <el-input size="mini" v-bind:value="SystemData.JointPos13" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节14位置</el-button>
                  <el-input size="mini" v-bind:value="SystemData.JointPos14" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节15位置</el-button>
                  <el-input size="mini" v-bind:value="SystemData.JointPos15" readonly/>
                </div>
              </el-col>
            </el-row>  
        </fieldset>
      </div>

      <div style="margin-top: 5px;">
        <fieldset style="background-color:#EBEEF5; border-color: white;"> 
          <legend style="font:8px; font-weight:800;  margin-left:15px; margin-right:15px; margin-bottom:10px;">电机信息</legend> 
            <el-row  style=" margin-left:15px; margin-right:15px;">
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机01电流</el-button>
                  <el-input v-bind:value="MotorData.Current01" readonly size="mini"/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机02电流</el-button>
                  <el-input v-bind:value="MotorData.Current02" readonly size="mini"/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机03电流</el-button>
                  <el-input size="mini" v-bind:value="MotorData.Current03" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机01故障</el-button>
                  <el-input size="mini" v-bind:value="MotorData.Error01" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机02故障</el-button>
                  <el-input size="mini" v-bind:value="MotorData.Error02" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机03故障</el-button>
                 <el-input size="mini" v-bind:value="MotorData.Error03" readonly/>
                </div>
              </el-col>
            </el-row>

            <el-row  style=" margin-left:15px; margin-right:15px;">
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机04电流</el-button>
                  <el-input v-bind:value="MotorData.Current04" readonly size="mini"/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机05电流</el-button>
                  <el-input size="mini" v-bind:value="MotorData.Current05 " readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机06电流</el-button>
                  <el-input size="mini" v-bind:value="MotorData.Current06" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机04故障</el-button>
                  <el-input size="mini" v-bind:value="MotorData.Error04" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机05故障</el-button>
                  <el-input size="mini" v-bind:value="MotorData.Error05" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机06故障</el-button>
                  <el-input size="mini" v-bind:value="MotorData.Error06" readonly/>
                </div>
              </el-col>
            </el-row>
            
            <el-row  style=" margin-left:15px; margin-right:15px;">
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机07电流</el-button>
                  <el-input v-bind:value="MotorData.Current07" readonly size="mini"/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机08电流</el-button>
                  <el-input size="mini" v-bind:value="MotorData.Current08" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机09电流</el-button>
                  <el-input size="mini" v-bind:value="MotorData.Current09" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机07故障</el-button>
                  <el-input size="mini" v-bind:value="MotorData.Error07" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机08故障</el-button>
                  <el-input size="mini" v-bind:value="MotorData.Error08" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机09故障</el-button>
                  <el-input size="mini" v-model="MotorData.Error09" readonly/>
                </div>
              </el-col>
            </el-row>

            <el-row  style=" margin-left:15px; margin-right:15px;">
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机10电流</el-button>
                  <el-input v-model="MotorData.Current10" readonly size="mini"/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机11电流</el-button>
                  <el-input size="mini" v-model="MotorData.Current11" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机12电流</el-button>
                  <el-input size="mini" v-model="MotorData.Current12" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机10故障</el-button>
                  <el-input size="mini" v-model="MotorData.Error10" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机11故障</el-button>
                  <el-input size="mini" v-bind:value="MotorData.Error11" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机12故障</el-button>
                  <el-input size="mini" v-bind:value="MotorData.Error12" readonly/>
                </div>
              </el-col>
            </el-row>

            <el-row  style=" margin-left:15px; margin-right:15px;">
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机13电流</el-button>
                  <el-input v-bind:value="MotorData.Current13" readonly size="mini"/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机14电流</el-button>
                  <el-input size="mini" v-bind:value="MotorData.Current14" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机15电流</el-button>
                  <el-input size="mini" v-bind:value="MotorData.Current15" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机13故障</el-button>
                  <el-input size="mini" v-bind:value="MotorData.Error13" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机14故障</el-button>
                  <el-input size="mini" v-bind:value="MotorData.Error14" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机15故障</el-button>
                  <el-input size="mini" v-bind:value="MotorData.Error15" readonly/>
                </div>
              </el-col>
            </el-row>



             <el-row  style=" margin-left:15px; margin-right:15px;">
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机01位置</el-button>
                  <el-input v-bind:value="MotorData.Current01" readonly size="mini"/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机02位置</el-button>
                  <el-input v-bind:value="MotorData.Current02" readonly size="mini"/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机03位置</el-button>
                  <el-input size="mini" v-bind:value="MotorData.Current03" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节01数据</el-button>
                  <el-input size="mini" v-bind:value="MotorData.Error01" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节02数据</el-button>
                  <el-input size="mini" v-bind:value="MotorData.Error02" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节03数据</el-button>
                 <el-input size="mini" v-bind:value="MotorData.Error03" readonly/>
                </div>
              </el-col>
            </el-row>

            <el-row  style=" margin-left:15px; margin-right:15px;">
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机04位置</el-button>
                  <el-input v-bind:value="MotorData.Current04" readonly size="mini"/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机05位置</el-button>
                  <el-input size="mini" v-bind:value="MotorData.Current05 " readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机06位置</el-button>
                  <el-input size="mini" v-bind:value="MotorData.Current06" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节04数据</el-button>
                  <el-input size="mini" v-bind:value="MotorData.Error04" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节05数据</el-button>
                  <el-input size="mini" v-bind:value="MotorData.Error05" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节06数据</el-button>
                  <el-input size="mini" v-bind:value="MotorData.Error06" readonly/>
                </div>
              </el-col>
            </el-row>
            
            <el-row  style=" margin-left:15px; margin-right:15px;">
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机07位置</el-button>
                  <el-input v-bind:value="MotorData.Current07" readonly size="mini"/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机08位置</el-button>
                  <el-input size="mini" v-bind:value="MotorData.Current08" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机09位置</el-button>
                  <el-input size="mini" v-bind:value="MotorData.Current09" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节07数据</el-button>
                  <el-input size="mini" v-bind:value="MotorData.Error07" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节08数据</el-button>
                  <el-input size="mini" v-bind:value="MotorData.Error08" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节09数据</el-button>
                  <el-input size="mini" v-model="MotorData.Error09" readonly/>
                </div>
              </el-col>
            </el-row>

            <el-row  style=" margin-left:15px; margin-right:15px;">
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机10位置</el-button>
                  <el-input v-model="MotorData.Current10" readonly size="mini"/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机11位置</el-button>
                  <el-input size="mini" v-model="MotorData.Current11" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机12位置</el-button>
                  <el-input size="mini" v-model="MotorData.Current12" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节10数据</el-button>
                  <el-input size="mini" v-model="MotorData.Error10" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节11数据</el-button>
                  <el-input size="mini" v-bind:value="MotorData.Error11" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节12数据</el-button>
                  <el-input size="mini" v-bind:value="MotorData.Error12" readonly/>
                </div>
              </el-col>
            </el-row>

            <el-row  style=" margin-left:15px; margin-right:15px;">
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机13位置</el-button>
                  <el-input v-bind:value="MotorData.Current13" readonly size="mini"/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机14位置</el-button>
                  <el-input size="mini" v-bind:value="MotorData.Current14" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机15位置</el-button>
                  <el-input size="mini" v-bind:value="MotorData.Current15" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节13数据</el-button>
                  <el-input size="mini" v-bind:value="MotorData.Error13" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节14数据</el-button>
                  <el-input size="mini" v-bind:value="MotorData.Error14" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节15数据</el-button>
                  <el-input size="mini" v-bind:value="MotorData.Error15" readonly/>
                </div>
              </el-col>
            </el-row>
          </fieldset>
      </div>

      <div style="margin-top: 5px;">
        <fieldset style="background-color:#EBEEF5; border-color: white;"> 
          <legend style="font:8px; font-weight:800;  margin-left:15px; margin-right:15px; margin-bottom:10px;">其他信息</legend> 
            <el-row  style=" margin-left:15px; margin-right:15px;">
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">驱动母线电压</el-button>
                  <el-input v-bind:value="FluorineData2.ExhaustGasTemp2 + TempIcon" readonly size="mini"/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">触觉1切向力</el-button>
                  <el-input
                    v-if="(FluorineData2.ExhaustGasProt2==='����' || FluorineData2.ExhaustGasProt2==='' || FluorineData2.ExhaustGasProt2===' / ')"
                    size="mini"
                    readonly
                    v-model="FluorineData2.ExhaustGasProt2"
                    
                  />
                  <el-input v-else size="mini" readonly v-model="FluorineData2.ExhaustGasProt2" WarningColor="warning"/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">触觉2切向力</el-button>
                  <el-input size="mini" v-bind:value="FluorineData2.EvaporatorTemp2 + TempIcon" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">触觉3切向力</el-button>
                  <el-input
                    v-if="(FluorineData2.EvaporatorProt2==='����' || FluorineData2.EvaporatorProt2==='' || FluorineData2.EvaporatorProt2===' / ')"
                    size="mini"
                    readonly
                    v-model="FluorineData2.EvaporatorProt2"
                    
                  />
                  <el-input v-else size="mini" readonly v-model="FluorineData2.EvaporatorProt2" WarningColor="warning"/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">触觉4切向力</el-button>
                  <el-input size="mini" v-bind:value="FluorineData2.CondenserTemp2 + TempIcon" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">触觉5切向力</el-button>
                  <el-input
                    v-if="(FluorineData2.CondenserProt2==='����'  || FluorineData2.CondenserProt2==='' || FluorineData2.CondenserProt2===' / ')"
                    size="mini"
                    readonly
                    v-model="FluorineData2.CondenserProt2"
                    
                  />
                  <el-input v-else size="mini" readonly v-model="FluorineData2.CondenserProt2" WarningColor="warning"/>
                </div>
              </el-col>
            </el-row>

            <el-row  style=" margin-left:15px; margin-right:15px;">
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">电机控制模式</el-button>
                  <el-input v-bind:value="FluorineData2.SuctionTemp2 + TempIcon" readonly size="mini"/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">触觉1法向力</el-button>
                  <el-input size="mini" v-bind:value="FluorineData2.LiquidPipeTemp2 + TempIcon" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">触觉2法向力</el-button>
                  <el-input size="mini" v-bind:value="FluorineData2.LowPress2 + barIcon" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">触觉3法向力</el-button>
                  <el-input size="mini" v-bind:value="FluorineData2.HighPress2 + barIcon" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">触觉4法向力</el-button>
                  <el-input
                    v-if="(FluorineData2.PressProt2==='����' || FluorineData2.PressProt2==='' || FluorineData2.PressProt2===' / ')"
                    size="mini"
                    readonly
                    v-model="FluorineData2.PressProt2"
                    
                  />
                  <el-input v-else size="mini" readonly v-model="FluorineData2.PressProt2" WarningColor="warning"/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">触觉5法向力</el-button>
                  <el-input
                    v-if="(FluorineData2.CompAcProt2==='����' || FluorineData2.CompAcProt2==='' || FluorineData2.CompAcProt2===' / ')"
                    size="mini"
                    readonly
                    v-model="FluorineData2.CompAcProt2"
                    
                  />
                  <el-input v-else size="mini" readonly v-model="FluorineData2.CompAcProt2" WarningColor="warning"/>
                </div>
              </el-col>
            </el-row>
            
            <el-row  style=" margin-left:15px; margin-right:15px;">
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">关节复位标志</el-button>
                  <el-input v-bind:value="FluorineData2.ReverseGasOverheat2 + TempIcon" readonly size="mini"/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">触觉1接近值</el-button>
                  <el-input size="mini" v-bind:value="FluorineData2.ExhaustGasOverheat2 + TempIcon" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">触觉2接近值</el-button>
                  <el-input size="mini" v-bind:value="FluorineData2.CondenserCasOverCool2 + TempIcon" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">触觉3接近值</el-button>
                  <el-input size="mini" v-bind:value="FluorineData2.TargetExhaustGas2 + TempIcon" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">触觉4接近值</el-button>
                  <el-input size="mini" v-bind:value="FluorineData2.TargetCondenserGas2 + TempIcon" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">触觉5接近值</el-button>
                  <el-input size="mini" v-model="FluorineData2.EEVStatus2" readonly/>
                </div>
              </el-col>
            </el-row>

            <el-row  style=" margin-left:15px; margin-right:15px;">
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">主控故障信息</el-button>
                  <el-input v-model="FluorineData2.EEVInitStep2" readonly size="mini"/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">触觉1切力方向</el-button>
                  <el-input size="mini" v-model="FluorineData2.EEVTargetStep2" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">触觉2切力方向</el-button>
                  <el-input size="mini" v-model="FluorineData2.EEVNowStep2" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">触觉3切力方向</el-button>
                  <el-input size="mini" v-model="FluorineData2.EEVAdjustStep2" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">触觉4切力方向</el-button>
                  <el-input size="mini" v-bind:value="FluorineData2.EEVAdjustPeriod2 + SecIcon" readonly/>
                </div>
              </el-col>
              <el-col :span="4">
                <div class="progress-box" >
                  <el-button type="text" size="small" style="width:170px; margin-right:3px;">触觉5切力方向</el-button>
                  <el-input size="mini" v-bind:value="FluorineData2.EEVAdjustTime2 + SecIcon" readonly/>
                </div>
              </el-col>
            </el-row>
          </fieldset>
      </div>
  </div>
</template>
<script>
import { ipcRenderer } from 'electron';
// import { setTimeout } from 'timers';
// import { EventBus } from "../../../../Utils/EventBus.js"
import { LogUtils } from '../../../../json/LogUtils'; 
import {
    // APP_EVENT_INIT_XLSX,
    // APP_EVENT_CLOSE_XLSX,
    APP_EVENT_OPEN_XLSX,
    // APP_EVENT_WRITE_XLSX,
    APP_EVENT_STOP_XLSX,
    // APP_EVENT_CLEAN_DATA,
  } from '../../../../js/constants/ElectronConstants'
  import {
    APP_REPORT_UART_RECV_DATA,
  } from '../../../../js/constants/IndoorConstants'
// import { constants } from 'fs';

export default {
  name: 'landing-page',
  computed: {
  },
  data() {
    return {
      SystemData: {
        SetJoint01: '',
        SetJoint02: '',
        SetJoint03: '',
        SetJoint04: '',
        SetJoint05: '',
        SetJoint06: '',
        SetJoint07: '',
        SetJoint08: '',
        SetJoint09: '',
        SetJoint10: '',
        SetJoint11: '',
        SetJoint12: '',
        SetJoint13: '',
        SetJoint14: '',
        SetJoint15: '',
        JointPos01: '',
        JointPos02: '',
        JointPos03: '',
        JointPos04: '',
        JointPos05: '',
        JointPos06: '',
        JointPos07: '',
        JointPos08: '',
        JointPos09: '',
        JointPos10: '',
        JointPos11: '',
        JointPos12: '',
        JointPos13: '',
        JointPos14: '',
        JointPos15: '',
      },
      
      MotorData: {
        Current01: '',
        Current02: '',
        Current03: '',
        Current04: '',
        Current05: '',
        Current06: '',
        Current07: '',
        Current08: '',
        Current09: '',
        Current10: '',
        Current11: '',
        Current12: '',
        Current13: '',
        Current14: '',
        Current15: '',
        Error01: '',
        Error02: '',
        Error03: '',
        Error04: '',
        Error05: '',
        Error06: '',
        Error07: '',
        Error08: '',
        Error09: '',
        Error10: '',
        Error11: '',
        Error12: '',
        Error13: '',
        Error14: '',
        Error15: '',
      },

      FluorineData2: {
        ExhaustGasTemp2: '',
        ExhaustGasProt2: '',
        EvaporatorTemp2: '',
        EvaporatorProt2: '',
        CondenserTemp2: '',
        CondenserProt2: '',
        SuctionTemp2: '',
        LiquidPipeTemp2: '',
        LowPress2: '',
        HighPress2: '',
        PressProt2: '',
        CompAcProt2: '',
        ReverseGasOverheat2: '',
        ExhaustGasOverheat2: '',
        CondenserCasOverCool2: '',
        TargetExhaustGas2: '',
        TargetCondenserGas2: '',
        EEVStatus2: '',
        EEVInitStep2: '',
        EEVTargetStep2: '',
        EEVNowStep2: '',
        EEVAdjustStep2: '',
        EEVAdjustPeriod2: '',
        EEVAdjustTime2: '',
        ReverseGasOverheatRate2: '',
        ExhaustGasOverheatRate2: '',
        WaterTempRate2: '',
        CompAdjustFreq2: '',
        CompAdjustPeriod2: '',
        CompRunStatus2: '',
        CompTargetFreq2: '',
        CompRunFreq2: '',
        CompIPMTemp2: '',
        CompACCurrent2: '',
        CompRunTime2: '',
        CompSoptTime2: '',
        FanTargetFreq2: '',
        FanRunFreq2: '',
        FanIPMTemp2: '',
        FanACCurrent2: '',
        FanRunTime2: '',
        FanSoptTime2: '',
      },
      ErrorData: {
        FluorineSystemErr1: '', 
        FluorineDriverErr1: '', 
        FluorineSystemErr2: '', 
        FluorineDriverErr2: '',
        WaterSystemErr: '', 
        WaterDriverErr: '', 
        SystemErr: '',
      },
      logHandle: null,
      nowTime: null,
      fileName: 'csv',
      csbStatue: 'close',
      currentStatue: false,

      TempIcon: '',
      AIcon: '',
      KPaIcon: '',
      barIcon: '',
      HzIcon: '',
      RateIcon: '',
      SecIcon: ''
    
    }

  },
  methods: {
      changelan () {
        this.$store.dispatch('ChangeLanFun')
      }, 
      refreshPortList () {
        ipcRenderer.send(IPC_CHANNEL_REFRESH_COM_LIST, 0)
      },
      startConnect () {
        ipcRenderer.send(IPC_CHANNEL_START_CONNECT, 0)
        this.currentStatue = true;
      },
      stopConnect () {
        ipcRenderer.send(IPC_CHANNEL_STOP_DOWNLOAD, 0)
        this.currentStatue = false;
      },
  },


  watch: {
    ['lang'](value) {
      if (value) {
          this.$i18n.locale = 'zh' 
          this.$store.dispatch('SetLocale', 'zh')
      } else {
          this.$i18n.locale = 'en'
          this.$store.dispatch('SetLocale', 'en')
      }

      this.OutdoorNG = ''
      this.IndoorNG = ''
    },
  },
  
  created: function () {

    ipcRenderer.on(APP_EVENT_OPEN_XLSX, (event, arg) => {
      if (this.$store.state.SystemData.MonitorMode === 'outdoor')
      {
        let jsonPath  //json·��
        let csvHead = [this.SystemData, this.MotorData, this.ErrorData, this.FluorineData2] 

        // console.log('test1', __dirname)
        // console.log('test2', this.$store.state.SystemData.csvFilePath)

        if (this.fileName !== this.$store.state.SystemData.OutcsvFilePath) {
          this.fileName = this.$store.state.SystemData.OutcsvFilePath
          jsonPath =  "./zhMap.json"  
          //jsonPath =  __dirname + "..\\..\\..\\..\\..\\json\\zhMap.json"
          this.logHandle = new LogUtils(this.fileName, jsonPath, csvHead);
        } else {
          //this.fileName = this.fileName
        }

        if ((this.logHandle === null) || (this.csbStatue==='close')) {
          
        } else {
          this.logHandle = this.logHandle
        } 

        this.csbStatue = 'open'
      }

    })

    //output EXcel
    ipcRenderer.on(APP_EVENT_STOP_XLSX, (event, arg) => {
      this.csbStatue = 'close'
    })

    //Serial Data 
    ipcRenderer.on(APP_REPORT_UART_RECV_DATA, (event, arg) => {
        let uint8ModbusData = [], uint16MudbusData = [], int16MudbusData = [];

        //console.log("recv:", arg)
        uint8ModbusData = arg.slice(0, arg.length - 2);
        uint8ModbusData = uint8ModbusData.slice(3);

        for (let i = 0; i < (arg[2]/2); i++) {
          uint16MudbusData[i] = ((uint8ModbusData[i*2] << 8) | (uint8ModbusData[i*2 + 1]))
          

          if ((i === (106-20)) || (i === (107-20)) || (i === (108-20)) || (i === (109-20)) || 
              (i === (88-20)) || (i === (89-20)) || (i === (95-20)) || (i === (96-20)) || (i ===(81-20)) || (i === (82-20))){
                //����ʱ��ֵ����ת���з���������
              int16MudbusData[i] = uint16MudbusData[i];
          }
          else{
            if(uint16MudbusData[i] & 0x8000) {
              int16MudbusData[i] = -(65536 - uint16MudbusData[i]);
            } else {
              int16MudbusData[i] = uint16MudbusData[i];
            }
          }
          
         
        }

        this.TempIcon = '��'
        this.AIcon = 'A'
        this.KPaIcon = 'kPa'
        this.barIcon = 'bar'
        this.HzIcon = 'Hz'
        this.RateIcon = '��/min'
        this.SecIcon = 's'


        //������Ϣ����
        this.ErrorData.FluorineSystemErr1 = '0x' + uint16MudbusData[3].toString(16);
        this.ErrorData.FluorineDriverErr1 = '0x' + uint16MudbusData[4].toString(16);
        this.ErrorData.FluorineSystemErr2 = '0x' + uint16MudbusData[5].toString(16); 
        this.ErrorData.FluorineDriverErr2 = '0x' + uint16MudbusData[6].toString(16);
        this.ErrorData.WaterSystemErr = '0x' + uint16MudbusData[7].toString(16);
        this.ErrorData.WaterDriverErr = '0x' + uint16MudbusData[8].toString(16);
        this.ErrorData.SystemErr = '0x' + uint16MudbusData[9].toString(16);

        if ((uint16MudbusData[4] & 0x100) && (uint16MudbusData[4] & 0x2000))
        {
          this.ErrorData.FluorineDriverErr1 = '0x' + uint16MudbusData[4].toString(16) + '(ѹ1:' + uint16MudbusData[122].toString() +  ')' + '(��1:' + uint16MudbusData[124].toString() +  ')';
        }
        else if (uint16MudbusData[4] & 0x100)
        {
          this.ErrorData.FluorineDriverErr1 = '0x' + uint16MudbusData[4].toString(16) + '(ѹ1:' + uint16MudbusData[122].toString() +  ')'; 
        }
        else if (uint16MudbusData[4] & 0x2000)
        {
          this.ErrorData.FluorineDriverErr1 = '0x' + uint16MudbusData[4].toString(16) + '(��1:' + uint16MudbusData[124].toString() +  ')';
        }

        if ((uint16MudbusData[6] & 0x100) && (uint16MudbusData[6] & 0x2000))
        {
          this.ErrorData.FluorineDriverErr2 = '0x' + uint16MudbusData[6].toString(16) + '(ѹ2:' + uint16MudbusData[123].toString() +  ')' + '(��2:' + uint16MudbusData[125].toString() +  ')';
        }
        else if (uint16MudbusData[6] & 0x100)
        {
          this.ErrorData.FluorineDriverErr2 = '0x' + uint16MudbusData[6].toString(16) + '(ѹ2:' + uint16MudbusData[123].toString() +  ')'; 
        }
        else if (uint16MudbusData[6] & 0x2000)
        {
          this.ErrorData.FluorineDriverErr2 = '0x' + uint16MudbusData[6].toString(16) + '(��2:' + uint16MudbusData[125].toString() +  ')';
        }

        if (uint16MudbusData[8] & 0x4)
        {
          this.ErrorData.WaterDriverErr = '0x' + uint16MudbusData[8].toString(16) + '(��:' + uint16MudbusData[126].toString() +  ')';
        }

        switch (int16MudbusData[30-20]) {
          case 0:
            this.SystemData.SetMode = '�ػ�'
            break;
          case 1:
            this.SystemData.SetMode = '�Զ�'
            break;
          case 2:
            this.SystemData.SetMode = 'ˮ��ѭ��'
            break;
          default:
            break;
        }

        switch (int16MudbusData[31-20]) {
          case 0:
            this.SystemData.RunMode = '�ػ�'
            break;
          case 1:
            this.SystemData.RunMode = '����'
            break;
          case 2:
            this.SystemData.RunMode = '����'
            break;
          case 3:
            this.SystemData.RunMode = 'ˮ��ѭ��'
            break;
          default:
            break;
        }

        this.SystemData.SetCool = (int16MudbusData[33-20] & 0xFF)  
        this.SystemData.SetHeat = (int16MudbusData[33-20] >> 8) 
        this.SystemData.CtrlTemp = int16MudbusData[34-20] / 10  
        switch (int16MudbusData[118-20]) {
          case 0:
            this.SystemData.CtrlMode = '��ˮ'
            break;
          case 1:
            this.SystemData.CtrlMode = '��ˮ'
            break;
          case 2:
            this.SystemData.CtrlMode = '��о'
            break;
          default:
            break;
        }
        this.SystemData.OutWaterTemp = int16MudbusData[36-20] / 10 
        this.SystemData.InWaterTemp = int16MudbusData[37-20] / 10 
        this.SystemData.OutWaterPress = int16MudbusData[67-20]
        this.SystemData.InWaterPress = int16MudbusData[68-20]
        this.SystemData.WaterTempDiff = Math.abs(((int16MudbusData[36-20] - int16MudbusData[37-20]) / 10)) 
        this.SystemData.WaterPressDiff = (int16MudbusData[67-20] - int16MudbusData[68-20]) 
        this.SystemData.AroundTemp = int16MudbusData[38-20] / 10 
        if (int16MudbusData[32-20] & 0x800)
        {
          this.SystemData.SysWaterTemp = int16MudbusData[35-20] / 10 
        }
        else 
        {
          this.SystemData.SysWaterTemp = ' / '
        }
        
        this.SystemData.PumpFreq =int16MudbusData[78-20] 
        this.SystemData.PumpCurrent = int16MudbusData[80-20] / 10 
        this.SystemData.PumpIPMTemp = int16MudbusData[83-20] / 10 
        this.SystemData.PumpRunTime = changetime(int16MudbusData[81-20]) 
        this.SystemData.Heater = (int16MudbusData[22-20]& (1<<0)) ? '����' : '�ر�'
        this.SystemData.WarningOut = (int16MudbusData[22-20] & (1<<11)) ? '����' : '�ر�'
        this.SystemData.CoolingFan = (int16MudbusData[22-20] & (1<<12)) ? '����' : '�ر�'
       
        if (int16MudbusData[32-20] & 0x3F3)
        {
          this.SystemData.ManualMode = '����' 
        }
        else 
        {
          this.SystemData.ManualMode = '�ر�' 
        }

        
        this.SystemData.OilReturn1 = (int16MudbusData[32-20] & (1<<2)) ? '����' : '�ر�'
        this.SystemData.OilReturn2 = (int16MudbusData[32-20] & (1<<3)) ? '����' : '�ر�'
        this.SystemData.HydraulicValve = (int16MudbusData[22-20] & (1<<4)) ? '����' : '�ر�'
        this.SystemData.WaterValve1 = (int16MudbusData[22-20] & (1<<1)) ? '����' : '�ر�'
        this.SystemData.WaterValve2 = (int16MudbusData[22-20] & (1<<2)) ? '����' : '�ر�'
        this.SystemData.WaterValve3 = (int16MudbusData[22-20] & (1<<3)) ? '����' : '�ر�'
        this.SystemData.OilHeatStrip1 = (int16MudbusData[22-20] & (1<<5)) ? '����' : '�ر�'
        this.SystemData.OilHeatStrip2 = (int16MudbusData[22-20] & (1<<6)) ? '����' : '�ر�'

        this.MotorData.ExhaustGasTemp1 = int16MudbusData[39-20] / 10 
        this.MotorData.ExhaustGasProt1 = '����'
        switch (int16MudbusData[20-20] & 0x07)
        {
          case 0:
            this.MotorData.ExhaustGasProt1 = '����'
            break;
          case 1:
            this.MotorData.ExhaustGasProt1 = '����'
            break;
          case 2:
            this.MotorData.ExhaustGasProt1 = '����'
            break;
          case 3:
            this.MotorData.ExhaustGasProt1 = '����'
            break;
          case 4:
            this.MotorData.ExhaustGasProt1 = '����'
            break;
          case 5:
            this.MotorData.ExhaustGasProt1 = '�콵'
            break;
          default:
            break;
        }
        this.MotorData.EvaporatorTemp1 = int16MudbusData[43-20] / 10 
        switch ((int16MudbusData[20-20] >> 3)& 0x07)
        {
          case 0:
            this.MotorData.EvaporatorProt1 = '����'
            break;
          case 1:
            this.MotorData.EvaporatorProt1 = '����'
            break;
          case 2:
            this.MotorData.EvaporatorProt1 = '����'
            break;
          case 3:
            this.MotorData.EvaporatorProt1 = '����'
            break;
          case 4:
            this.MotorData.EvaporatorProt1 = '����'
            break;
          case 5:
            this.MotorData.EvaporatorProt1 = '�콵'
            break;
          default:
            break;
        }

        this.MotorData.CondenserTemp1 = int16MudbusData[42-20] / 10
        this.MotorData.CondenserProt1 = '����'
        switch ((int16MudbusData[20-20] >> 6)& 0x07)
        {
          case 0:
            this.MotorData.CondenserProt1 = '����'
            break;
          case 1:
            this.MotorData.CondenserProt1 = '����'
            break;
          case 2:
            this.MotorData.CondenserProt1 = '����'
            break;
          case 3:
            this.MotorData.CondenserProt1 = '����'
            break;
          case 4:
            this.MotorData.CondenserProt1 = '����'
            break;
          case 5:
            this.MotorData.CondenserProt1 = '�콵'
            break;
          default:
            break;
        }

        this.MotorData.SuctionTemp1 = int16MudbusData[40-20] / 10 
        this.MotorData.LiquidPipeTemp1 = int16MudbusData[41-20] / 10 
        this.MotorData.LowPress1 = int16MudbusData[70-20] / 10 
        this.MotorData.HighPress1 = int16MudbusData[69-20] / 10 
        switch ((int16MudbusData[20-20] >> 9)& 0x07)
        {
          case 0:
            this.MotorData.PressProt1 = '����'
            break;
          case 1:
            this.MotorData.PressProt1 = '����'
            break;
          case 2:
            this.MotorData.PressProt1 = '����'
            break;
          case 3:
            this.MotorData.PressProt1 = '����'
            break;
          case 4:
            this.MotorData.PressProt1 = '����'
            break;
          case 5:
            this.MotorData.PressProt1 = '�콵'
            break;
          default:
            break;
        }

        switch ((int16MudbusData[20-20] >> 12)& 0x07)
        {
          case 0:
            this.MotorData.CompAcProt1 = '����'
            break;
          case 1:
            this.MotorData.CompAcProt1 = '����'
            break;
          case 2:
            this.MotorData.CompAcProt1 = '����'
            break;
          case 3:
            this.MotorData.CompAcProt1 = '����'
            break;
          case 4:
            this.MotorData.CompAcProt1 = '����'
            break;
          case 5:
            this.MotorData.CompAcProt1 = '�콵'
            break;
          default:
            break;
        }
        this.MotorData.ReverseGasOverheat1 = int16MudbusData[49-20] / 10 
        this.MotorData.ExhaustGasOverheat1 = int16MudbusData[51-20] / 10 
        this.MotorData.CondenserCasOverCool1 = int16MudbusData[53-20] / 10 
        this.MotorData.TargetExhaustGas1 = int16MudbusData[112-20] / 10
        this.MotorData.TargetCondenserGas1 = int16MudbusData[114-20] /10
        switch (int16MudbusData[55-20])
        {
          case 0:
            this.MotorData.EEVStatus1 = '��λ'
            break;
          case 1:
            this.MotorData.EEVStatus1 = 'ֹͣ'
            break;
          case 2:
            this.MotorData.EEVStatus1 = '����'
            break;
          case 3:
            this.MotorData.EEVStatus1 = '����'
            break;
          case 4:
            this.MotorData.EEVStatus1 = '����'
            break;
          case 5:
            this.MotorData.EEVStatus1 = '�̶�'
            break;
          case 6:
            this.MotorData.EEVStatus1 = 'ͻ��'
            break;
          case 7:
            this.MotorData.EEVStatus1 = '���'
            break;
          case 8:
            this.MotorData.EEVStatus1 = '�ֶ�'
            break;
          default:
            break;
        }
        this.MotorData.EEVInitStep1 = int16MudbusData[59-20] 
        this.MotorData.EEVTargetStep1 = int16MudbusData[61-20] 
        this.MotorData.EEVNowStep1 = int16MudbusData[63-20]
        this.MotorData.EEVAdjustStep1 = int16MudbusData[65-20]
        this.MotorData.EEVAdjustPeriod1 = int16MudbusData[57-20] 
        this.MotorData.EEVAdjustTime1 = int16MudbusData[116-20] 
        this.MotorData.ReverseGasOverheatRate1 = int16MudbusData[130-20] / 10
        this.MotorData.ExhaustGasOverheatRate1 = int16MudbusData[132-20] / 10
        this.MotorData.WaterTempRate1 = int16MudbusData[134-20] / 10
        this.MotorData.CompAdjustFreq1 = int16MudbusData[136-20]
        this.MotorData.CompAdjustPeriod1 = int16MudbusData[138-20] 
        switch (int16MudbusData[140-20])
        {
          case 0:
            this.MotorData.CompRunStatus1 = '����'
            break;
          case 1:
            this.MotorData.CompRunStatus1 = '����'
            break;
          case 2:
            this.MotorData.CompRunStatus1 = 'ж��'
            break;
          default:
            break;
        }
        this.MotorData.CompTargetFreq1 = int16MudbusData[84-20] 
        this.MotorData.CompRunFreq1 = int16MudbusData[85-20] 
        this.MotorData.CompIPMTemp1 = int16MudbusData[90-20] / 10 
        this.MotorData.CompACCurrent1 = int16MudbusData[87-20] / 10 
        this.MotorData.CompRunTime1 = changetime(int16MudbusData[88-20]) 
        this.MotorData.CompSoptTime1 = changetime(int16MudbusData[89-20]) 
        this.MotorData.FanTargetFreq1 = int16MudbusData[98-20]  
        this.MotorData.FanRunFreq1 = int16MudbusData[99-20] 
        this.MotorData.FanIPMTemp1 = int16MudbusData[102-20] / 10 
        this.MotorData.FanACCurrent1 = int16MudbusData[124-20] / 10 
        this.MotorData.FanRunTime1 = changetime(int16MudbusData[106-20]) 
        this.MotorData.FanSoptTime1 = changetime(int16MudbusData[108-20]) 

        //��ϵͳ2��Ϣ
        if (int16MudbusData[32-20] & 0x400)
        {
          this.FluorineData2.ExhaustGasTemp2 = int16MudbusData[44-20] / 10 
          this.FluorineData2.ExhaustGasProt2 = '����'
          switch (int16MudbusData[21-20] & 0x07)
          {
            case 0:
              this.FluorineData2.ExhaustGasProt2 = '����'
              break;
            case 1:
              this.FluorineData2.ExhaustGasProt2 = '����'
              break;
            case 2:
              this.FluorineData2.ExhaustGasProt2 = '����'
              break;
            case 3:
              this.FluorineData2.ExhaustGasProt2 = '����'
              break;
            case 4:
              this.FluorineData2.ExhaustGasProt2 = '����'
              break;
            case 5:
              this.FluorineData2.ExhaustGasProt2 = '�콵'
              break;
            default:
              break;
          }
          this.FluorineData2.EvaporatorTemp2 = int16MudbusData[48-20] / 10 
          switch ((int16MudbusData[21-20] >> 3)& 0x07)
          {
            case 0:
              this.FluorineData2.EvaporatorProt2 = '����'
              break;
            case 1:
              this.FluorineData2.EvaporatorProt2 = '����'
              break;
            case 2:
              this.FluorineData2.EvaporatorProt2 = '����'
              break;
            case 3:
              this.FluorineData2.EvaporatorProt2 = '����'
              break;
            case 4:
              this.FluorineData2.EvaporatorProt2 = '����'
              break;
            case 5:
              this.FluorineData2.EvaporatorProt2 = '�콵'
              break;
            default:
              break;
          }

          this.FluorineData2.CondenserTemp2 = int16MudbusData[47-20] / 10
          this.FluorineData2.CondenserProt2 = '����'
          switch ((int16MudbusData[21-20] >> 6)& 0x07)
          {
            case 0:
              this.FluorineData2.CondenserProt2 = '����'
              break;
            case 1:
              this.FluorineData2.CondenserProt2 = '����'
              break;
            case 2:
              this.FluorineData2.CondenserProt2 = '����'
              break;
            case 3:
              this.FluorineData2.CondenserProt2 = '����'
              break;
            case 4:
              this.FluorineData2.CondenserProt2 = '����'
              break;
            case 5:
              this.FluorineData2.CondenserProt2 = '�콵'
              break;
            default:
              break;
          }

          this.FluorineData2.SuctionTemp2 = int16MudbusData[45-20] / 10 
          this.FluorineData2.LiquidPipeTemp2 = int16MudbusData[46-20] / 10 
          this.FluorineData2.LowPress2 = int16MudbusData[74-20] / 10 
          this.FluorineData2.HighPress2 = int16MudbusData[73-20] / 10 
          switch ((int16MudbusData[21-20] >> 9)& 0x07)
          {
            case 0:
              this.FluorineData2.PressProt2 = '����'
              break;
            case 1:
              this.FluorineData2.PressProt2 = '����'
              break;
            case 2:
              this.FluorineData2.PressProt2 = '����'
              break;
            case 3:
              this.FluorineData2.PressProt2 = '����'
              break;
            case 4:
              this.FluorineData2.PressProt2 = '����'
              break;
            case 5:
              this.FluorineData2.PressProt2 = '�콵'
              break;
            default:
              break;
          }

          switch ((int16MudbusData[21-20] >> 12)& 0x07)
          {
            case 0:
              this.FluorineData2.CompAcProt2 = '����'
              break;
            case 1:
              this.FluorineData2.CompAcProt2 = '����'
              break;
            case 2:
              this.FluorineData2.CompAcProt2 = '����'
              break;
            case 3:
              this.FluorineData2.CompAcProt2 = '����'
              break;
            case 4:
              this.FluorineData2.CompAcProt2 = '����'
              break;
            case 5:
              this.FluorineData2.CompAcProt2 = '�콵'
              break;
            default:
              break;
          }
          this.FluorineData2.ReverseGasOverheat2 = int16MudbusData[50-20] / 10 
          this.FluorineData2.ExhaustGasOverheat2 = int16MudbusData[52-20] / 10 
          this.FluorineData2.CondenserCasOverCool2 = int16MudbusData[54-20] / 10 
          this.FluorineData2.TargetExhaustGas2 = int16MudbusData[113-20] / 10
          this.FluorineData2.TargetCondenserGas2 = int16MudbusData[115-20] / 10
          switch (int16MudbusData[56-20])
          {
            case 0:
              this.FluorineData2.EEVStatus2 = '��λ'
              break;
            case 1:
              this.FluorineData2.EEVStatus2 = 'ֹͣ'
              break;
            case 2:
              this.FluorineData2.EEVStatus2 = '����'
              break;
            case 3:
              this.FluorineData2.EEVStatus2 = '����'
              break;
            case 4:
              this.FluorineData2.EEVStatus2 = '����'
              break;
            case 5:
              this.FluorineData2.EEVStatus2 = '�̶�'
              break;
            case 6:
              this.FluorineData2.EEVStatus2 = 'ͻ��'
              break;
            case 7:
              this.FluorineData2.EEVStatus2 = '���'
              break;
            case 8:
              this.FluorineData2.EEVStatus2 = '�ֶ�'
              break;
            default:
              break;
          }

          this.FluorineData2.EEVInitStep2 = int16MudbusData[60-20] 
          this.FluorineData2.EEVTargetStep2 = int16MudbusData[62-20] 
          this.FluorineData2.EEVNowStep2 = int16MudbusData[64-20]
          this.FluorineData2.EEVAdjustStep2 = int16MudbusData[66-20]
          this.FluorineData2.EEVAdjustPeriod2 = int16MudbusData[58-20]  
          this.FluorineData2.EEVAdjustTime2 = int16MudbusData[117-20]  
          this.FluorineData2.ReverseGasOverheatRate2 = int16MudbusData[131-20] / 10
          this.FluorineData2.ExhaustGasOverheatRate2 = int16MudbusData[133-20] / 10
          this.FluorineData2.WaterTempRate2 = int16MudbusData[135-20] / 10
          this.FluorineData2.CompAdjustFreq2 = int16MudbusData[137-20]
          this.FluorineData2.CompAdjustPeriod2 = int16MudbusData[139-20]
          switch (int16MudbusData[141-20])
          {
            case 0:
              this.MotorData.CompRunStatus2 = '����'
              break;
            case 1:
              this.MotorData.CompRunStatus2 = '����'
              break;
            case 2:
              this.MotorData.CompRunStatus2 = 'ж��'
              break;
            default:
              break;
          }
    
          this.FluorineData2.CompTargetFreq2 = int16MudbusData[91-20] 
          this.FluorineData2.CompRunFreq2 = int16MudbusData[92-20] 
          this.FluorineData2.CompIPMTemp2 = int16MudbusData[97-20] / 10 
          this.FluorineData2.CompACCurrent2 = int16MudbusData[94-20] / 10 
          this.FluorineData2.CompRunTime2 = changetime(int16MudbusData[95-20]) 
          this.FluorineData2.CompSoptTime2 = changetime(int16MudbusData[96-20]) 
          this.FluorineData2.FanTargetFreq2 = int16MudbusData[100-20]  
          this.FluorineData2.FanRunFreq2 = int16MudbusData[101-20] 
          this.FluorineData2.FanIPMTemp2 = int16MudbusData[103-20] / 10 
          this.FluorineData2.FanACCurrent2 = int16MudbusData[125-20] / 10 
          this.FluorineData2.FanRunTime2 = changetime(int16MudbusData[107-20]) 
          this.FluorineData2.FanSoptTime2 = changetime(int16MudbusData[109-20]) 
        }
        else 
        {
          this.FluorineData2.ExhaustGasTemp2 = ' / ' 
          this.FluorineData2.ExhaustGasProt2 = ' / '
          this.FluorineData2.ExhaustGasProt2 = ' / '
          this.FluorineData2.EvaporatorTemp2 = ' / ' 
          this.FluorineData2.EvaporatorProt2 = ' / '
          this.FluorineData2.CondenserTemp2 = ' / '
          this.FluorineData2.CondenserProt2 = ' / '
          this.FluorineData2.CondenserProt2 = ' / '
          this.FluorineData2.SuctionTemp2 = ' / ' 
          this.FluorineData2.LiquidPipeTemp2 = ' / '
          this.FluorineData2.LowPress2 = ' / '
          this.FluorineData2.HighPress2 = ' / '
          this.FluorineData2.PressProt2 = ' / '
          this.FluorineData2.CompAcProt2 = ' / '
          this.FluorineData2.ReverseGasOverheat2 = ' / ' 
          this.FluorineData2.ExhaustGasOverheat2 = ' / '
          this.FluorineData2.CondenserCasOverCool2 = ' / '
          this.FluorineData2.TargetExhaustGas2 = ' / '
          this.FluorineData2.TargetCondenserGas2 = ' / '
          this.FluorineData2.EEVStatus2 = ' / '
          this.FluorineData2.EEVInitStep2 = ' / '
          this.FluorineData2.EEVTargetStep2 = ' / '
          this.FluorineData2.EEVNowStep2 = ' / '
          this.FluorineData2.EEVAdjustStep2 = ' / '
          this.FluorineData2.EEVAdjustPeriod2 = ' / ' 
          this.FluorineData2.EEVAdjustTime2 = ' / '
          this.FluorineData2.ReverseGasOverheatRate2 = ' / '
          this.FluorineData2.ExhaustGasOverheatRate2 = ' / '
          this.FluorineData2.WaterTempRate2 = ' / '
          this.FluorineData2.CompAdjustFreq2 = ' / '
          this.FluorineData2.CompAdjustPeriod2 = ' / '
          this.FluorineData2.CompRunStatus2 = ' / '
          this.FluorineData2.CompTargetFreq2 = ' / '
          this.FluorineData2.CompRunFreq2 = ' / '
          this.FluorineData2.CompIPMTemp2 = ' / '
          this.FluorineData2.CompACCurrent2 = ' / '
          this.FluorineData2.CompRunTime2 = ' / '
          this.FluorineData2.CompSoptTime2 = ' / '
          this.FluorineData2.FanTargetFreq2 = ' / '
          this.FluorineData2.FanRunFreq2 = ' / '
          this.FluorineData2.FanIPMTemp2 = ' / '
          this.FluorineData2.FanACCurrent2 = ' / '
          this.FluorineData2.FanRunTime2 = ' / '
          this.FluorineData2.FanSoptTime2 = ' / '
        }

        //д���������
        if (this.nowTime !== new Date().toLocaleString()){
          this.nowTime = new Date().toLocaleString()
          
          var TempTimeStr24 = new Date();
          if (this.csbStatue === 'open') {
            this.logHandle.WriteDecoderLog(TempTimeStr24.toLocaleString('chinese', {hour12:false}));
          }
        }


    })

    function changetime(value) {
	        var secondTime = parseInt(value);
	        var minuteTime = 0;
	        var hourTime = 0;
	        if(secondTime > 60) {
	            minuteTime = parseInt(secondTime / 60);
	            secondTime = parseInt(secondTime % 60);
	            if(minuteTime > 60) {
	                hourTime = parseInt(minuteTime / 60);
	                minuteTime = parseInt(minuteTime % 60);
	            }
	        }
	        var time = "" + parseInt(secondTime) + "s";
 
	        if(minuteTime > 0) {
	        	time = "" + parseInt(minuteTime) + ":" + time;
	        }
	        if(hourTime > 0) {
	        	time = "" + parseInt(hourTime) + ":" + time;
	        }
	        return time;
        }

  },
  beforeDestroy(){
    ipcRenderer.send(IPC_CHANNEL_STOP_DOWNLOAD, 0)
  }

}
</script scoped>
<style >
.conter {
  margin: 4px;
  background-color:#ffffff;
}
.serial {
  margin-bottom:5dx;
  margin-top:5dx;
}
.version-fie {
  box-sizing: border-box;
  height: 100%;
}
.indoor {
  flex: 2.7;
  background-color: #d7e4f2;
  margin-top: 4px;
  padding-bottom: 5px;
}

.myicon-refresh {
  font-size: 30px;
  cursor: pointer;
}
@keyframes refresh {
    0% {
        transform: rotate(0deg)
    }
    50% {
        transform: rotate(180deg)
    }
    100% {
        transform: rotate(360deg)
    }
}
.myicon-refresh.animate {
    animation: refresh 2s infinite;
}

.progress-box {
  display: flex;
  align-items: center;
  font-size: 15px;
  height: 30px;
  font-family: "Helvetica Neue";
}

.el-input__inner[DangerColor="danger"] {
  background-color:red;
}

.el-input__inne {
  background-color:#ffffff;
}

.el-input__inner[WarningColor="warning"] {
  background-color: #E6A23C;
}

.el-input__inner[SuccessColor="success"] {
  background-color: #67C23A;
}

.el-textarea__inner {
  background-color:#ffffff !important;
  font-size: 13px !important;
  padding: 2px !important;
  color: red !important;
}


.el-hanler {
  padding: 5px !important;
  background-color: #606266;
}


.el-select {
  
  height:32px !important;
}

.el-input__inner {
   height:24px !important;
   border-radius:0px !important;
   color:#222222 !important;
   font-size: 12px !important;
}

.el-button--text {
  color:black !important;
}
.el-input__icon {
  line-height:30px  !important;
}

.line {
    height: 5px;
    background: #ba55d3
}
.el-button--text {
  color:black;
}
.my-main legend{
    font-size: 14px;
    height: 14px !important;
    padding-bottom: 3px;
  }
  .my-main .el-col-4{
    height: 26px !important;
  }
  .my-main .el-col-4 .progress-box{
    height: 18px; 
  }
  .my-main .el-tabs__nav .el-tabs__item{
  height: 35px;
  font-weight: 800;
}
</style>




