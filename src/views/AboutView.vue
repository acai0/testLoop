<template>
    <div id="app">
    <br> <br/>
        <h3>Test</h3>
        <div class="container">
            <div v-for='index in 100' :key='index'>
                <!-- <strong>5 * {{index}}  = {{index*5}}</strong> -->
                  <div class="accordion" id="accordionFlushExample">
        <div class="accordion-item">
          <h2 class="accordion-header" id="myTable">
            <button
              class="accordion-button collapsed"
              type="button"
              data-bs-toggle="collapse"
              data-bs-target="#flush-collapseOne"
              aria-expanded="false"
              aria-controls="flush-collapseOne"
            >
              VLC
            </button>
          </h2>
          <div
            id="flush-collapseOne"
            class="accordion-collapse collapse"
            aria-labelledby="flush-headingOne"
            data-bs-parent="#accordionFlushExample"
          >
            <div class="accordion-body">
                <table class="table table-condensed table-striped">
              <tr >
                <th>OS</th>
                <th>Paquet</th>
                <th>Version</th>
                <th>Option</th>
                <th>Ensure</th>
              </tr>

              <tr id="windows">
                <td>
                  <i
                    class="bi bi-windows"
                    v-b-popover.hover.top="'Windows'"
                  ></i>
                </td>
                <td>vlc</td>
                <td><i class="bi bi-unlock-fill" v-b-popover.hover.top="'Version maintenue'"/>7.12.3</td>
                <td><code>[--param --verbs]</code></td>
                <td><code>present</code></td>
              </tr>

              <tr id="ubuntu">
                <td>
                  <i
                    class="bi bi-box2-fill"
                    v-b-popover.hover.top="'Ubuntu'"
                  ></i>
                </td>
                <td>vlc</td>
                <td><i class="bi bi-arrow-repeat" v-b-popover.hover.top="'Mise à jour automatique'"/>7.12.3</td>
                <td></td>
                <td><code>latest</code></td>
              </tr>

              <tr id="macos">
                <td>
                  <i class="bi bi-apple" v-b-popover.hover.top="'MacOS'"></i>
                </td>
                <td>vlc</td>
                <td><i class="bi bi-lock-fill" v-b-popover.hover.top="'Version non maintenue'"/>7.12.3</td>
                <td></td>
                <td></td>
              </tr>
                  </table>
            </div>
          </div>
        </div>
    </div>
            </div>
        
        

  </div>
  </div>
  </div>
</template>
<script>
</script>