<template>
  <div id="app">
    <div class="main">
      <div class="con">
        <div class="n1">
          <div class="daimond" style="position: relative;" width="140" height="140">
            <a class="shape" href="http://tdzk.net/ship_move.php?MoveTo=-1995070771">
              <img class="shape s1" src="./assets/nav-up.gif" alt="9106" title="9106">
            </a>
            <a href="http://tdzk.net/ship_move.php?MoveTo=-1694060108">
              <img class="shape s3" src="./assets/nav-left.gif" alt="9125" title="9125">
            </a>
            <a @click="toggel1">
              <img
                class="shape s4"
                src="./assets/nav-dropscout0.gif"
                alt="Sector 9126"
                title="Sector 9126"
              >
            </a>
            <a href="http://tdzk.net/ship_move.php?MoveTo=-152858542">
              <img class="shape s5" src="./assets/nav-right.gif" alt="9127" title="9127">
            </a>
            <a href="getChief.php?level=0">
              <img class="shape s6" src="./assets/nav-center.gif" alt>
            </a>
            <a href="http://tdzk.net/ship_move.php?MoveTo=454878741">
              <img class="shape s7" src="./assets/nav-down.gif" alt="9146" title="9146">
            </a>
            <a href="http://tdzk.net/ship_move.php?MoveTo=108468389">
              <img
                class="shape s2"
                src="./assets/nav-jumpnode.gif"
                alt="Jump Node: 42001"
                title="Jump Node: 42001"
              >
            </a>
          </div>
          <div class="center" style="position: relative;">
            <a href="http://tdzk.net/repair_process.php?Turns=1&amp;VeriCode=395338472">
              <img
                src="./assets/repair.gif"
                height="25"
                width="25"
                border="0"
                alt="Repair 1 Turn"
                title="Repair 1 Turn"
              >
            </a>
            <br>
            <a href="http://tdzk.net/repair_process.php?RepairEMP=1&amp;VeriCode=395338472">
              <img
                src="./assets/repair2.gif"
                height="25"
                width="25"
                border="0"
                alt="Repair EMP"
                title="Repair EMP"
              >
            </a>
          </div>
          <div class="center1">
            <input class="navbarinput" type="text" name="target" value="9126" size="6">
            <input
              type="image"
              src="http://tdzk.agadak.net/getChief/getChief_files/plot.gif"
              height="20"
              width="30"
              border="0"
              alt="Plot Course"
              title="Plot Course"
              javascript
              document.plotform.submit
            >
          </div>
          <div class="center2">
            <a href="http://tdzk.net/view_reports.php?Display=1">
              <img
                src="./assets/combat.gif"
                height="21"
                width="29"
                border="0"
                alt="Combat Reports"
                title="Combat Reports"
              >
            </a>

            <a href="http://tdzk.net/view_reports.php?Display=3">
              <img
                src="./assets/planet.gif"
                height="21"
                width="29"
                border="0"
                alt="Planet Reports"
                title="Planet Reports"
              >
            </a>

            <a href="http://tdzk.net/view_reports.php?Display=2">
              <img
                src="./assets/forces.gif"
                height="21"
                width="29"
                border="0"
                alt="Force Reports"
                title="Force Reports"
              >
            </a>

            <a href="http://tdzk.net/alliance_forum.php">
              <img
                src="./assets/forum.gif"
                height="21"
                width="29"
                border="0"
                alt="Alliance Forum Posts"
                title="Alliance Forum Posts"
              >
            </a>
            <v-badge v-model="show" color="cyan" right>
              <template v-slot:badge>
                <span>6</span>
              </template>
              <a href="http://tdzk.net/view_messages.php">
                <img
                  src="./assets/messages.gif"
                  height="21"
                  width="29"
                  border="0"
                  alt="Messages"
                  title="Messages"
                >
              </a>
            </v-badge>
          </div>
        </div>
        <div style="display: flex;height: -webkit-fill-available;position: relative;">
          <div class="n2 n" :class="{ex}">
            <div>
              <!-- end of Dividing Blue line -->
              <span class="pri">Level: 49</span>
              <br>
              <br>
              <el-progress :text-inside="true" :stroke-width="18" :percentage="70"></el-progress>
              <br>
              <!-- <span class="high">EXP:</span><br/> -->
              <div class="high" align="left">XP: 553,180,173</div>
              <!-- <span class="quad">Next:</span><br/> -->
              <div class="quad" align="left">NL: 588,245,000</div>
              <div class="high" align="left">Alignment: -91</div>

              <div class="ter" align="left">$2,326,487,750</div>
              <div class="sec" align="left">Turns: 2666</div>
              <!-- Dividing Blue line -->
              <hr>
              <br>�
              <br>
              <!-- end of Dividing Blue line -->
              Galactic Time:
              <br>06:37:46 EST
              <br>
              <!-- Dividing Blue line -->
              <br>
              <hr>
              <br>�
              <br>
              <!-- end of Dividing Blue line -->

              <strong>�</strong>
              <a href="http://tdzk.net/system_map.php?id=9" target="_sysmap">System Map</a>
              <br>
              <strong>�</strong>
              <a href="http://tdzk.net/view_nav.php">Navigation</a>
              <br>
              <strong>�</strong>
              <a href="http://tdzk.net/galaxy_map.php">Galaxy Map</a>
              <br>
              <br>
              <strong>�</strong>
              <a href="http://tdzk.net/view_news.php">News</a>
              <br>
              <strong>�</strong>
              <a href="http://tdzk.net/view_news.php?Display=1">Notices</a>
              <br>
              <br>
              <strong>�</strong>
              <a href="http://tdzk.net/online_players.php">Online Players</a>
              <br>
              <br>
              <strong>�</strong>
              <a href="http://tdzk.net/stats_options.php">Stats/Options</a>
              <br>
              <strong>�</strong>
              <a href="http://tdzk.net/alliance_roster.php">Alliance</a>
              <br>
              <strong>�</strong>
              <a href="http://tdzk.net/alliances.php">Alliance List</a>
              <br>
              <strong>�</strong>
              <a href="http://tdzk.net/bounties.php">Bounties</a>
              <br>
              <strong>�</strong>
              <a href="http://tdzk.net/rankings.php">Rankings</a>
              <br>
              <br>
              <strong>�</strong>
              <a href="http://tdzk.net/view_forces.php">Forces</a>
              <br>
              <strong>�</strong>
              <a href="http://tdzk.net/view_planets.php">Planets</a>
              <br>
              <br>
              <strong>�</strong>
              <a href="http://forums.tdzk.com/" target="_webboard">Web Board</a>
              <br>
              <br>
              <strong>�</strong>
              <a href="http://tdzk.net/help/" target="_help">Help</a>
              <br>
              <strong>�</strong>
              <a href="http://tdzk.net/logout.php">Logout</a>
              <br>
            </div>
          </div>
          <div class="n3 n">
            <div class="center1">
              <span class="pagetitle">Current Sector</span>
              <br>Sector 9126
              <br>
            </div>
            <div class="center2">
              <span>Deep Space</span>
              <br>
              <span>Normal</span>
              <br>
              <a href="javascript:helpPopup('Term', 'Auras')">
                <img src="./assets/aura_title.gif" height="13" width="40" border="0" alt>
              </a>
            </div>
          </div>
          <div class="ico">
            <a @click="toggel">
              <i class="fas fa-bars fa-3x"></i>
            </a>
          </div>
          <div class="mid">
            <div class="m1 m">
              <div class="pri" style="font-weight: bold; text-decoration: underline;">Messages:</div>
              <div align="center">
                <span class="screenmessage">
                  Level 0 (2250ms Examine || 1250ms Attack)
                  <br>
                </span>
              </div>
            </div>
            <div class="m2 m">
              <div class="mr10">
                <img class="star" src="./assets/stars100.gif" border="0" alt>
              </div>
              <div>
                <strong>Sector</strong>
                <br>
                <span class="pagetitle">
                  <strong>9126</strong>
                </span>
                <br>
                <span class="high">Deep Space</span>
                <br>
                <span class="quad">Normal</span>
                <br>
                <span class="quad">100% Visibility</span>
                <br>
                <a href="javascript:helpPopup('Term', 'Auras')">
                  <img src="./assets/aura_title.gif" height="13" width="40" border="0" alt>
                </a>
              </div>
              <div class="e3">
                <span class="pri">
                  <a href="http://tdzk.net/ship_move.php?MoveTo=-1995070771">[9106]</a>
                </span>
                <br>|
                <br>
                <span class="pri">
                  <a href="http://tdzk.net/ship_move.php?MoveTo=-1694060108">[9125]-</a>
                </span>
                <span class="quad">[9126]-</span>
                <span class="pri">
                  <a href="http://tdzk.net/ship_move.php?MoveTo=-152858542">[9127]</a>
                </span>
                <br>|
                <br>
                <span class="pri">
                  <a href="http://tdzk.net/ship_move.php?MoveTo=454878741">[9146]</a>
                </span>
                ---
                <span class>
                  <a href="http://tdzk.net/ship_move.php?MoveTo=108468389">[42001]</a>
                </span>
              </div>
            </div>
            <div class="m3 m">
              <span class="pagetitle" style="font-weight: bold;">Concentric Station</span>
              <br>
              <span class="pagetitle">Port Concentric</span>
              <br>
              <span class="quad">Alignment: 0</span>
              <br>
              <span class="quad">Level: 5</span>
              <br>
              <span class="big">
                [
                <a href="http://tdzk.net/dock_to_port.php?Auth=2049823320">DOCK</a>] [
                <a href="http://tdzk.net/">RAID</a>]
              </span>
            </div>
            <div class="m4">
              <v-layout align-center justify-center row fill-height>
                <v-flex xs12>
                  <h3>Other Ships in this Sector</h3>
                </v-flex>
              </v-layout>
              <v-layout class="body-1 head" row>
                <v-flex xs3>
                  <h4>Name</h4>
                </v-flex>
                <v-flex xs3>
                  <h4>Class/Race</h4>
                </v-flex>
                <v-flex xs3>
                  <h4>Level</h4>
                </v-flex>
                <v-flex xs3>
                  <h4>Rating</h4>
                </v-flex>
              </v-layout>
              <v-layout row>
                <v-flex xs3>
                  <h5>Flying Gamecube</h5>
                </v-flex>
                <v-flex xs3>
                  <h4>Ranger</h4>
                </v-flex>
                <v-flex xs3>
                  <h4>L: 225</h4>
                </v-flex>
                <v-flex xs3>
                  <h4>5/9</h4>
                </v-flex>
              </v-layout>
              <v-layout row>
                <v-flex xs3>
                  <span class="alert">
                    Mardak
                    <span class="sec">[Online]</span>
                  </span>
                </v-flex>
                <v-flex xs3>
                  <h4>Wraith</h4>
                </v-flex>
                <v-flex xs3>
                  <h4>L: 27</h4>
                </v-flex>
                <v-flex xs3>
                  <span class="pri">
                    [
                    <a
                      href="/getChief/getChief.php?Message=Mardak slaps you&lt;br&gt;for examining him.&lt;br&gt;&lt;span class='alert'&gt;DIEEE!!&lt;/span&gt;&amp;level=0"
                    >Examine</a>]
                  </span>
                </v-flex>
              </v-layout>
              <v-layout row>
                <v-flex xs12>
                  <a href="http://tdzk.net/alliance_roster.php?Display=575">
                    <img
                      title="unAdmin unAlliance"
                      alt="unAdmin unAlliance"
                      src="http://tdzk.agadak.net/getChief/getChief_files/alliance-575.gif"
                      border="0"
                    >
                  </a>
                  <a href="http://tdzk.net/examine_remote.php?id=19">
                    <img
                      title="Master Chief"
                      alt="Master Chief"
                      src="./assets/player-19.gif"
                      border="0"
                    >
                  </a>
                </v-flex>
              </v-layout>
            </div>
            <div class="m5 m">
              <v-layout row>
                <v-flex xs12 class="text-center">
                  <span class="subtitle">Sector Resources:</span>
                </v-flex>
              </v-layout>
              <v-layout row>
                <v-flex xs6>
                  <span>Machinery:</span>
                </v-flex>
                <v-flex xs3>
                  <span>10390</span>
                </v-flex>
                <v-flex xs3>
                  <span class="ter">
                    [
                    <a href="http://tdzk.net/current_sector.php?Good=7&amp;Action=1">Gather</a>]
                    <br>[
                    <a href="http://tdzk.net/current_sector.php?Good=7&amp;Action=2">Gather All</a>]
                  </span>
                </v-flex>
              </v-layout>
              <v-layout row>
                <v-flex xs6>
                  <span>Electronics:</span>
                </v-flex>
                <v-flex xs3>
                  <span>5255</span>
                </v-flex>
                <v-flex xs3>
                  <span class="ter">
                    [
                    <a href="http://tdzk.net/current_sector.php?Good=8&amp;Action=1">Gather</a>]
                    <br>[
                    <a href="http://tdzk.net/current_sector.php?Good=8&amp;Action=2">Gather All</a>]
                  </span>
                </v-flex>
              </v-layout>
            </div>
          </div>
        </div>
      </div>
      <div class="con1" :class="{conex}">
        <div class="n1" :class="{ex1}">
          Best Viewed at 800 x 600 or Higher Resolution
          <br>Taenaria Derivia Zallus Kitara 2.1 � 2003 Vivid
          <br>
        </div>
        <div class="n2" :class="{ex2}">
          <span class="pri">SHD: 625/625</span>
          <br>
          <span class="pri">ARM: 6875/6875</span>
          <br>
          <span class="pri">POW: 300/300</span>
          <br>
          <span class="pri">EMP: 0/1000</span>
          <br>
          <a href="http://tdzk.net/view_ship.php">Details</a>
          <strong>�</strong>
          <br>
          <a href="http://tdzk.net/repair.php">Repair</a>
          <strong>�</strong>
          <br>
          <br>
          <!-- Dividing Blue line -->
          <hr>
          <br>�
          <!-- end of Dividing Blue line -->
          <span class="pri">Level: 250</span>
          <br>Rating:
          <br>
          <span class="pri">65/75</span>
          <br>Speed: 14
          <br>Maneuver: 70
          <br>
          <a href="http://tdzk.net/view_equipment.php">Equipment</a>
          <strong>�</strong>
          <br>

          <!-- Dividing Blue line -->
          <br>
          <hr>
          <br>�
          <br>
          <!-- end of Dividing Blue line -->

          <a href="http://tdzk.net/view_cargo.php">Ship Cargo</a>
          <strong>�</strong>
          <br>
          <br>0 Total Holds
          <br>

          <!-- Dividing Blue line -->
          <br>
          <hr>
          <br>�
          <br>
          <!-- end of Dividing Blue line -->

          <a href="http://tdzk.net/view_weapons.php">Weapons</a>
          <strong>�</strong>
          <br>Primary:
          <br>[1]
          <span class="sec">25GC</span>
          <br>[2]
          <span class="sec">25GC</span>
          <br>[3]
          <span class="sec">25GC</span>
          <br>[4]
          <span class="sec">25GC</span>
          <br>
          <br>Secondary:
          <br>[1]
          <span class="sec">ResDM</span> 33
          <br>[2]
          <span class="sec">ResDM</span> 33
          <br>[3]
          <span class="sec">ResDM</span> 33
          <br>[4]
          <span class="sec">ResDM</span> 33
          <br>[5]
          <span class="sec">ResDM</span> 33
          <br>[6]
          <span class="sec">ResDM</span> 33
          <br>
          <br>
          <br>TComp Lvl:
          <span class="sec">0</span>
          <br>DAmp �Lvl:
          <span class="sec">0</span>
          <br>Weapon Mode:
          <br>
          <span class="sec">All/No Evade</span>
          <br>

          <!-- Dividing Blue line -->
          <br>
          <hr>
          <br>�
          <br>
          <!-- end of Dividing Blue line -->

          <a href="http://tdzk.net/view_drones.php">Drones</a>
          <strong>�</strong>
          <br>
          <br>
          <span style="color: rgb(0, 128, 0);">Repair: 50</span>
          <br>
          <span class="quad">Hangars: 50</span>
          <br>
          <span class="quad">Empty: 0</span>
          <br>
          <!-- Dividing Blue line -->
          <br>
          <hr>
          <br>�
          <!-- end of Dividing Blue line -->

          <div style="text-align: right;">Squadron:</div>
          <form action="change_frequency.php" method="post">
            <input type="submit" name="Frequency" class="small" style="width: 12px;" value="X">
            <input type="submit" name="Frequency" class="small" style="width: 12px;" value="1">
            <input
              type="submit"
              name="Frequency"
              class="small"
              style="border: 1px solid rgb(0, 153, 51); width: 12px;"
              value="2"
            >
            <input type="submit" name="Frequency" class="small" style="width: 12px;" value="3">
            <input type="submit" name="Frequency" class="small" style="width: 12px;" value="4">
          </form>

          <!-- Dividing Blue line -->
          <hr>
          <br>�
          <br>
          <!-- end of Dividing Blue line -->

          <a href="http://tdzk.net/set_deploy.php">Deploy</a>
          <strong>�</strong>
          <br>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "app",
  components: {},
  data() {
    return {
      ex: false,
      ex1: false,
      ex2: false,
      conex: false,
      show: true
    };
  },
  methods: {
    toggel: function() {
      if ((this.ex = true)) {
        this.ex = false;
      }
      this.ex1 = !this.ex1;
      this.ex2 = !this.ex2;
      this.conex = !this.conex;
    },
    toggel1: function() {
      if (this.ex1 == true && this.ex2 == true && this.conex == true) {
        this.ex1 = false;
        this.ex2 = false;
        this.conex = false;
      }
      this.ex = !this.ex;
    }
  }
};
</script>
<style >
@import "../dist/css/main.min.css";
@import "../dist/css/style1.min.css";
@import "../dist/css/style2.min.css";
@import "../dist/css/style3.min.css";
</style>
