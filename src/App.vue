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
            <a @click="ex=!ex">
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
              <table border="0" cellspacing="0" cellpading="2">
                <tbody>
                  <tr>
                    <td class="mainblock" rowspan="3">
                      <img src="./assets/stars100.gif" height="100" width="100" border="0" alt>
                    </td>
                    <td class="mainblock" width="10" rowspan="3">
                      <img src="./assets/spacer.gif" height="1" width="10" border="0" alt>
                    </td>
                    <td
                      width="100"
                      class="mainblock"
                      rowspan="3"
                      style="text-align: left; vertical-align: middle;"
                    >
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
                      <table class="mainblock" border="0" cellpadding="0" cellspacing="0">
                        <tbody>
                          <tr style="text-align: right;">
                            <td width="40" height="13">
                              <a href="javascript:helpPopup('Term', 'Auras')">
                                <img
                                  src="./assets/aura_title.gif"
                                  height="13"
                                  width="40"
                                  border="0"
                                  alt
                                >
                              </a>
                            </td>
                          </tr>
                        </tbody>
                      </table>
                    </td>

                    <td class="mainblock" width="10" rowspan="3">
                      <img src="./assets/spacer.gif" height="1" width="10" border="0" alt>
                    </td>
                    <td
                      class="mainblock"
                      width="33"
                      style="text-align: center; vertical-align: bottom;"
                    >
                      <img src="./assets/spacer.gif" height="1" width="33" border="0" alt>
                    </td>
                    <td class="mainblock" style="text-align: center; vertical-align: middle;">
                      <span class="pri">
                        [
                        <a href="http://tdzk.net/ship_move.php?MoveTo=-1995070771">9106</a>]
                      </span>
                      <br>|
                    </td>
                    <td class="mainblock" style="text-align: center; vertical-align: bottom;"></td>
                  </tr>
                  <tr height="34">
                    <td class="mainblock" style="text-align: center; vertical-align: middle;">
                      <span class="pri">
                        <a href="http://tdzk.net/ship_move.php?MoveTo=-1694060108">[9125]-</a>
                      </span>
                    </td>
                    <td class="mainblock" style="text-align: center; vertical-align: middle;">
                      <span class="quad">[9126]</span>
                    </td>
                    <td class="mainblock" style="text-align: center; vertical-align: middle;">
                      -
                      <span class="pri">
                        [
                        <a href="http://tdzk.net/ship_move.php?MoveTo=-152858542">9127</a>]
                      </span>
                    </td>
                  </tr>
                  <tr height="33">
                    <td class="mainblock" style="text-align: center; vertical-align: top;"></td>
                    <td class="mainblock" style="text-align: center; vertical-align: middle;">
                      |
                      <br>
                      <span class="pri">
                        [
                        <a href="http://tdzk.net/ship_move.php?MoveTo=454878741">9146</a>]
                      </span>
                    </td>
                    <td class="mainblock" style="text-align: center; vertical-align: top;">
                      <span class>
                        [
                        <a href="http://tdzk.net/ship_move.php?MoveTo=108468389">42001</a>]
                      </span>
                    </td>
                  </tr>
                </tbody>
              </table>
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
              <table class="table-chart-bordered" border="0" cellspacing="0" cellpadding="0">
                <tbody>
                  <tr>
                    <td width="200"></td>
                    <td width="150"></td>
                    <td width="70"></td>
                    <td width="40"></td>
                    <td width="60"></td>
                  </tr>
                  <tr class="alt1">
                    <td
                      class="subtitle"
                      colspan="5"
                      style="vertical-align: bottom; text-align: center;"
                    >Other Ships in this Sector</td>
                  </tr>
                  <tr class="alt0">
                    <td></td>
                    <td align="left">Name</td>
                    <td align="left">Class/Race</td>
                    <td align="left">Level</td>
                    <td>Rating</td>
                  </tr>
                  <tr>
                    <td class="spacer" colspan="5" height="1"></td>
                  </tr>
                  <tr class="alt1">
                    <td width="200" height="20">
                      <a href="http://tdzk.net/alliance_roster.php?Display=575">
                        <img
                          title="unAdmin unAlliance"
                          alt="unAdmin unAlliance"
                          src="http://tdzk.agadak.net/getChief/getChief_files/alliance-575.gif"
                          border="0"
                          height="20"
                          width="50"
                        >
                      </a>
                      <a href="http://tdzk.net/examine_remote.php?id=19">
                        <img
                          title="Master Chief"
                          alt="Master Chief"
                          src="./assets/player-19.gif"
                          height="20"
                          width="150"
                          border="0"
                        >
                      </a>
                    </td>
                    <td align="left">K for Kan't spell</td>
                    <td align="left">Freighter</td>
                    <td align="left">L: 215</td>
                    <td>5/9</td>
                  </tr>
                  <tr class="alt1">
                    <td align="left">
                      <table border="0" cellspacing="2" cellpadding="0" class="alt1">
                        <tbody>
                          <tr height="13">
                            <td></td>
                          </tr>
                        </tbody>
                      </table>
                    </td>
                    <td align="left">
                      <span class>
                        Master Chief
                        <span class="sec">[Online]</span>
                      </span>
                    </td>
                    <td align="left">Tamaran</td>
                    <td align="left">L: 27</td>
                    <td>
                      <span class="pri">
                        [
                        <a href="javascript:examineChief()">Examine</a>]
                      </span>
                    </td>
                  </tr>
                  <tr>
                    <td class="spacer" colspan="5" height="1"></td>
                  </tr>
                  <tr class="alt1">
                    <td width="200" height="20">
                      <a href="http://tdzk.net/alliance_roster.php?Display=571">
                        <img
                          title="Admin Alliance"
                          alt="Admin Alliance"
                          src="http://tdzk.agadak.net/getChief/getChief_files/alliance-571.gif"
                          border="0"
                          height="20"
                          width="50"
                        >
                      </a>
                      <a href="http://tdzk.net/examine_remote.php?id=1">
                        <img
                          title="Aelanna"
                          alt="Aelanna"
                          src="./assets/player-1.gif"
                          height="20"
                          width="150"
                          border="0"
                        >
                      </a>
                    </td>
                    <td align="left">TPx Feathered Ven...</td>
                    <td align="left">Escape Pod</td>
                    <td align="left">L: 215</td>
                    <td>5/9</td>
                  </tr>
                  <tr class="alt1">
                    <td align="left">
                      <table border="0" cellspacing="2" cellpadding="0" class="alt1">
                        <tbody>
                          <tr height="13">
                            <td></td>
                          </tr>
                        </tbody>
                      </table>
                    </td>
                    <td align="left">
                      <span class="ter">
                        Aelanna
                        <span class="sec">[Online]</span>
                      </span>
                    </td>
                    <td align="left">Taenarian</td>
                    <td align="left">L: 1</td>
                    <td>
                      <span class="pri">
                        <!--        [<a href="/getChief/getChief.php?Message=That doesn't look like chief to me!<script>alert('Nope')</script>&level=0">Examine</a>] -->
                        [
                        <a
                          href="/getChief/getChief.php?Message=That doesn't look like chief to me!&amp;level=0"
                        >Examine</a>]
                      </span>
                    </td>
                  </tr>
                </tbody>
              </table>
            </div>
            <div class="m5 m">
              <table width="390" class="mainblock" border="0" cellspacing="0" cellpadding="2">
                <tbody>
                  <tr>
                    <td colspan="3" style="text-align: center;">
                      <span class="subtitle">Sector Resources:</span>
                    </td>
                  </tr>
                  <tr>
                    <td width="150" style="text-align: left; vertical-align: top;">Machinery:</td>
                    <td width="100" style="text-align: right; vertical-align: top;">10390</td>
                    <td width="140" style="text-align: right; vertical-align: top;">
                      <span class="ter">
                        [
                        <a href="http://tdzk.net/current_sector.php?Good=7&amp;Action=1">Gather</a>]
                        [
                        <a
                          href="http://tdzk.net/current_sector.php?Good=7&amp;Action=2"
                        >Gather All</a>]
                      </span>
                    </td>
                  </tr>
                  <tr>
                    <td width="150" style="text-align: left; vertical-align: top;">Electronics:</td>
                    <td width="100" style="text-align: right; vertical-align: top;">5255</td>
                    <td width="140" style="text-align: right; vertical-align: top;">
                      <span class="ter">
                        [
                        <a href="http://tdzk.net/current_sector.php?Good=8&amp;Action=1">Gather</a>]
                        [
                        <a
                          href="http://tdzk.net/current_sector.php?Good=8&amp;Action=2"
                        >Gather All</a>]
                      </span>
                    </td>
                  </tr>
                </tbody>
              </table>
            </div>
          </div>
        </div>
      </div>
      <div class="con1">
        <div class="n1">
          Best Viewed at 800 x 600 or Higher Resolution
          <br>Taenaria Derivia Zallus Kitara 2.1 � 2003 Vivid
          <br>
        </div>
        <div class="n2">
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
      show: true
    };
  },
  methods: {}
};
</script>
<style >
@import '../dist/css/main.min.css';
</style>
