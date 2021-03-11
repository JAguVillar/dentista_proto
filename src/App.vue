<template>
  <div id="app">
    <div style="display: flex;">
      <HelloWorld
        style="margin-right: 10px; margin-left: 10px;"
        :top="Math.floor(Math.random() * 3)"
        :right="Math.floor(Math.random() * 3)"
        :bottom="Math.floor(Math.random() * 3)"
        :left="Math.floor(Math.random() * 3)"
        :center="Math.floor(Math.random() * 3)"
      />
      <!-- <svg
        width="210mm"
        height="297mm"
        version="1.1"
        viewBox="0 0 210 297"
        xmlns="http://www.w3.org/2000/svg"
        xmlns:cc="http://creativecommons.org/ns#"
        xmlns:dc="http://purl.org/dc/elements/1.1/"
        xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#"
      >
        <metadata>
          <rdf:RDF>
            <cc:Work rdf:about="">
              <dc:format>image/svg+xml</dc:format>
              <dc:type rdf:resource="http://purl.org/dc/dcmitype/StillImage" />
              <dc:title />
            </cc:Work>
          </rdf:RDF>
        </metadata>
        <g>
          <g
            transform="translate(-1.0424 3.2456)"
            fill="#fff"
            stroke="#000"
            stroke-linecap="round"
            stroke-linejoin="round"
          >
            <rect
              x="61.342"
              y="100.55"
              width="89.401"
              height="89.401"
              stroke-width="2.6458"
            />
            <path
              transform="scale(.26458)"
              d="m179.02 327.22 52.396 52.395h338.75l52.396-52.395z"
              stroke-width="10"
            />
            <path
              d="m164.72 86.577-13.863 13.863v89.628l13.863 13.863z"
              stroke-width="2.6458"
            />
            <path
              d="m47.365 203.93 13.863-13.863h89.628l13.863 13.863z"
              stroke-width="2.6458"
            />
            <path
              d="m47.365 203.93 13.863-13.863v-89.628l-13.863-13.863z"
              stroke-width="2.6458"
            />
          </g>
        </g>
        <g>
          <path
            d="m42.496 85.996 125.01 125.01m0-125.01-125.01 125.01"
            fill="none"
            stroke="#dc2625"
            stroke-linecap="round"
            stroke-width="7.9375"
          />
        </g>
      </svg> -->
    </div>
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
  },
};
</script>

<style>
#app {
  height: 100vh;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
    background: #eaeefa;
}
</style>
