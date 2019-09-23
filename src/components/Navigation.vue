<template>
  <header id="Navigation">
    <input id="nav-input" type="checkbox" class="nav-unshown">
    <a id="logo" href="./index">
        <svg class="logo-svg" version="1.1" x="0px" y="0px" width="40px" height="40px" viewBox="0 0 50 50">
        <path stroke-miterlimit="10" d="M6.167,0H5C2.239,0,0,2.239,0,5v40c0,2.762,2.239,5,5,5h1.167V0z"/>
            <path stroke-miterlimit="10" d="M45,0H9.167v7.209
                c1.788-2.106,4.228-3.41,6.917-3.41c5.469,0,9.917,5.372,9.917,11.975c0,0.829-0.671,1.5-1.5,1.5s-1.5-0.671-1.5-1.5
                c0-4.949-3.103-8.975-6.917-8.975s-6.917,4.026-6.917,8.975V50h13.835V33c0-0.828,0.671-1.5,1.5-1.5s1.5,0.672,1.5,1.5v4.626
                L40.754,26.31c0.656-0.505,1.599-0.38,2.104,0.277c0.504,0.657,0.38,1.599-0.277,2.104l-11.47,8.799L43.621,50H45
                c2.762,0,5-2.238,5-5V5C50,2.239,47.762,0,45,0z M30.734,23.946c-0.821,1.722-6.232,5.047-6.232,5.047s-5.411-3.325-6.232-5.047
                c-0.82-1.721-0.09-3.782,1.631-4.602s3.781-0.091,4.601,1.631h0.002c0.819-1.722,2.88-2.451,4.601-1.631
                S31.555,22.225,30.734,23.946z"/>
        </svg>
    </a>
    <label id="nav-open" for="nav-input">
        <svg id="menu" class="menu-svg" version="1.1" x="0px" y="0px" width="40px" height="40px" viewBox="0 0 50 50">
            <line stroke-miterlimit="10" x1="8.125" y1="11.855" x2="41.875" y2="11.855"/>
            <line stroke-miterlimit="10" x1="8.125" y1="25" x2="41.875" y2="25"/>
            <line stroke-miterlimit="10" x1="8.125" y1="38.146" x2="41.875" y2="38.146"/>
        </svg>
    </label>
      <label class="nav-unshown" id="nav-close" for="nav-input"></label>
      <div id="nav-content">
        <div id="nav-content-innner">
      <label id="closebutton" for="nav-input">
        <svg class="close-svg" version="1.1" x="0px" y="0px" width="40px" height="40px" viewBox="0 0 50 50">
            <line stroke-miterlimit="10" x1="8.125" y1="11.854" x2="41.875" y2="38.146"/>
            <line stroke-miterlimit="10" x1="8.125" y1="38.145" x2="41.875" y2="11.855"/>
        </svg>
      </label>
          <ul>
            <li><label class="menuTag" v-scroll-to="'#top'" @click="clearcheck">Top</label></li>
            <li><label class="menuTag" v-scroll-to="'#skills'" @click="clearcheck">Skill</label></li>
            <li><label class="menuTag" v-scroll-to="'#profile'" @click="clearcheck">Profile</label></li>
          </ul>
          <label>
          <a href="https://github.com/rik8kir8rik8">
              <svg class="sns-icon" version="1.1" x="0px" y="0px" width="30px" height="30px" viewBox="0 0 60 60">
                <path stroke-miterlimit="10"  d="M27.134,34.861c1.74-0.424,3.444-0.734,5.085-1.26
                  c2.048-0.66,3.831-1.834,5.074-3.707c0.457-0.684,1.01-0.85,1.746-0.787c2.729,0.227,5.459,0.428,8.29,0.645
                  c0.058-0.213,0.136-0.502,0.286-1.059c-3.095-0.275-6.056-0.541-9.044-0.807c-0.182-0.916,0.424-1.059,1.097-1.055
                  c2.161,0.006,4.319,0.033,6.479,0.064c0.466,0.006,0.932,0.061,1.426,0.098c0.47-0.955,0.04-1.209-0.749-1.219
                  c-2.003-0.019-4.006-0.035-6.007-0.053c-0.568-0.003-1.136,0-1.825,0c0-0.529-0.021-0.949,0.004-1.365
                  c0.104-1.799-0.24-3.492-1.189-5.004c-0.378-0.604-0.395-1.115-0.268-1.822c0.258-1.439,0.433-2.925,0.387-4.383
                  c-0.057-1.817-0.743-2.338-2.438-1.867c-1.247,0.344-2.442,0.943-3.597,1.559c-0.603,0.32-1.056,0.461-1.748,0.225
                  c-3.452-1.18-6.935-1.162-10.387,0.02c-0.678,0.232-1.164,0.188-1.736-0.26c-1.15-0.901-2.465-1.432-3.903-1.646
                  c-1.368-0.205-1.91,0.076-2.034,1.488c-0.111,1.294-0.148,2.656,0.122,3.91c0.284,1.313,0.197,2.368-0.473,3.534
                  c-0.823,1.429-1.067,3.067-0.961,4.744c0.017,0.261,0.003,0.522,0.003,0.95c-0.766,0-1.433-0.018-2.098,0.004
                  c-1.894,0.063-3.787,0.145-5.682,0.213c-0.578,0.018-0.908,0.215-0.649,0.988c1.542,0,3.106-0.004,4.672,0.002
                  c1.105,0.006,2.216-0.02,3.317,0.061c0.368,0.025,0.718,0.336,1.076,0.518c-0.033,0.1-0.067,0.201-0.101,0.301
                  c-2.901,0.275-5.805,0.549-8.778,0.83c0.025,0.465,0.042,0.766,0.061,1.084c3.127-0.258,6.152-0.51,9.256-0.768
                  c2.588,4.094,6.56,5.248,10.927,5.664c-0.954,0.953-1.876,1.914-2.851,2.814c-0.254,0.232-0.666,0.328-1.02,0.383
                  c-0.831,0.129-1.672,0.189-2.508,0.295c-2.188,0.273-3.859-0.566-5.227-2.359c-0.602-0.787-1.488-1.35-2.294-1.947
                  c-0.243-0.18-0.646-0.127-1.104-0.029c1.758,1.557,2.195,3.795,3.154,5.738c0.66,1.344,1.867,1.879,3.267,1.92
                  c1.357,0.041,2.716,0.01,4.204,0.01c0,2.5,0.076,4.838-0.027,7.168c-0.061,1.359-0.968,1.869-2.18,1.35
                  C7.323,46.244,1.867,39.516,0.313,29.633C-1.837,15.975,6.993,2.95,20.164,0.261c13.578-2.773,26.189,6.22,29.168,19.503
                  c2.839,12.656-3.458,25.168-14.973,30.063c-2.04,0.867-2.752,0.367-2.786-2.002c-0.022-1.475-0.015-2.951-0.004-4.43
                  C31.594,39.732,30.272,36.82,27.134,34.861z"/>
              </svg>
              </a>
            </label>
            <label><a href="https://twitter.com/rik_kir_study">
              <svg class="sns-icon" version="1.1" x="0px" y="0px" width="30px" height="30px" viewBox="0 1 55 55" >
                <path fill="" d="M49.648,25.315C49.648,38.953,38.603,50,24.964,50S0.279,38.953,0.279,25.315
                  c0-13.639,11.046-24.685,24.685-24.685S49.648,11.676,49.648,25.315z M20.446,38.336c10.948,0,16.935-9.071,16.935-16.934
                  c0-0.258,0-0.518-0.013-0.765c1.16-0.84,2.173-1.889,2.975-3.085c-1.062,0.469-2.209,0.79-3.419,0.938
                  c1.234-0.74,2.172-1.901,2.617-3.296c-1.148,0.679-2.42,1.173-3.777,1.444c-1.086-1.16-2.629-1.876-4.345-1.876
                  c-3.282,0-5.949,2.666-5.949,5.949c0,0.469,0.049,0.926,0.16,1.358c-4.95-0.247-9.332-2.617-12.269-6.221
                  c-0.506,0.876-0.802,1.901-0.802,2.987c0,2.062,1.049,3.888,2.654,4.95c-0.975-0.025-1.888-0.296-2.69-0.741
                  c0,0.024,0,0.049,0,0.074c0,2.888,2.048,5.282,4.776,5.838c-0.494,0.136-1.024,0.21-1.567,0.21c-0.383,0-0.753-0.037-1.123-0.111
                  c0.753,2.37,2.95,4.085,5.554,4.135c-2.036,1.593-4.604,2.542-7.393,2.542c-0.482,0-0.951-0.023-1.419-0.085
                  C13.954,37.349,17.09,38.336,20.446,38.336"/>
                </svg>
              </a>
            </label>
        </div>
      </div>
</header>
</template>

<script>
export default {
  name: 'Navigation',
  props: {
    msg: String
  },
  components: {
  },
  methods: {
      clearcheck: function(){
      var checkbox = document.getElementById( "nav-input" );
      checkbox.checked = false;
    }
  }
}
</script>

<style lang="scss">
ul{
  list-style: none;
  label{
    cursor:pointer;
    font-family: Muli, cursive;
    color:#616161;
    &:hover{
      color:#E9E29B;
      transition: 0.5s ease-in-out;
      margin-left:1rem;
    }
  }
}
  #Navigation{
    position: relative;
  }

  .nav-unshown {
    display:none;
  }

  #logo{
    position:fixed;
    margin-left:-10%;
      &:hover .logo-svg{
        fill:#72B0AF;
        transition: 0.5s ease-in-out;
      }
      .logo-svg{
        float:right;
        fill:#616161;
        stroke: #000; 
        stroke-dasharray: 2000;
        stroke-dashoffset: 0;
        stroke-width: 0.5;
      }
  }

  #menu{
    position:fixed;
  }
  .menu-svg{
      stroke:#616161;
      stroke-width:2.5;
      stroke-linecap:round;
      &:hover{
        background:#72B0AF;
        transition: 0.5s ease-in-out;
      }
  }
  .menuTag{
    font-family:Noto Serif;
  }

  .sns-icon{
    fill:#616161;
    stroke:none;
          &:hover{
        background:#72B0AF;
        transition: 0.5s ease-in-out;
      }
  }

  #nav-open {
    float:right;
    position: relative;
    display: inline-block;
    cursor:pointer;
  }

  #nav-close {
    display: none;
    position: fixed;
    z-index: 99;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: black;
    opacity: 0;
    transition: .3s ease-in-out;
  }

  #closebutton{
    position: relative;
    top: 10%;
    left: 90%;
    display: inline-block;
    vertical-align: middle;
    cursor:pointer;
  }

  .close-svg{
      stroke:#616161;
      stroke-width:2.5;
      stroke-linecap:round;
        &:hover {
          background:#E9E29B;
          transition: 0.5s ease-in-out;
       }
  }

  @media screen and (min-width: 600px) {
  #nav-content {
    overflow: auto;
    position: fixed;
    top: 0;
    left: 0;
    z-index: 9999;
    width: 40%;
    min-width: 300px;
    height: 100%;
    background: #72B0AF;
    transition: .3s ease-in-out;
    -webkit-transform: translateX(250%);
    transform: translateX(250%);
    opacity:0.8;
  }
  #nav-input:checked ~ #nav-content {
    -webkit-transform: translateX(150%);
    transform: translateX(150%);
    box-shadow: -6px 0 10px rgba(0,0,0,.25);
  }
    #nav-content-innner {
      padding:10%;
    }
  }

  @media screen and (max-width: 600px) {
  #nav-content {
    overflow: auto;
    position: fixed;
    top: 0;
    left: 0;
    z-index: 9999;
    width: 90%;
    max-width: 600px;
    height: 100%;
    background: #72B0AF;
    transition: .3s ease-in-out;
    -webkit-transform: translateX(115%);
    transform: translateX(115%);
    opacity:0.8;
  }
  #nav-input:checked ~ #nav-content {
    -webkit-transform: translateX(15%);
    transform: translateX(15%);
    box-shadow: -6px 0 10px rgba(0,0,0,.25);
  }
    .innner {
      padding:50%;
    }
  }

  @media screen and (max-width: 479px) {
  #nav-content {
    overflow: auto;
    position: fixed;
    top: 0;
    left: 0;
    z-index: 9999;
    width: 90%;
    max-width: 479px;
    height: 100%;
    background: #72B0AF;
    transition: .3s ease-in-out;
    -webkit-transform: translateX(115%);
    transform: translateX(115%);
    opacity:0.8;
  }
  #nav-input:checked ~ #nav-content {
    -webkit-transform: translateX(15%);
    transform: translateX(15%);
    box-shadow: -6px 0 10px rgba(0,0,0,.25);
  }
      #nav-content-innner {
      margin-right:10%;
    }
    .close-svg {
      background:#E9E29B;
      }
  }

  #nav-input:checked ~ #nav-close {
    display: block;
    opacity: .5;
  }
</style>