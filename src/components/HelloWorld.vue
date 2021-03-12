<template>
  <div class="hello">
    <svg
      width="30mm"
      height="30mm"
      version="1.1"
      viewBox="0 0 120 120"
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
      <g
        transform="translate(-46.043 -85.255)"
        fill="#fff"
        stroke="#6b7380"
        stroke-linecap="round"
        stroke-linejoin="round"
      >
        <rect
          x="61.342"
          y="100.55"
          width="89.401"
          height="89.401"
          stroke-width="2.6458"
          :fill="dienteCenter == '0' ? '#ffffff' : dienteCenter == '1' ? '#fba5a4' : '#92c5fc'"
          @click="clickCenter"
        />
        <path
          transform="scale(.26458)"
          d="m179.02 327.22 52.396 52.395h338.75l52.396-52.395z"
          stroke-width="10"
          :fill="dienteTop == '0' ? '#ffffff' : dienteTop == '1' ? '#fba5a4' : '#92c5fc'"
          @click="clickTop"
        />
        <path
          d="m164.72 86.577-13.863 13.863v89.628l13.863 13.863z"
          stroke-width="2.6458"
          :fill="dienteRight == '0' ? '#ffffff' : dienteRight == '1' ? '#fba5a4' : '#92c5fc'"
          @click="clickRight"
        />
        <path
          d="m47.365 203.93 13.863-13.863h89.628l13.863 13.863z"
          stroke-width="2.6458"
          :fill="dienteBottom == '0' ? '#ffffff' : dienteBottom == '1' ? '#fba5a4' : '#92c5fc'"
          @click="clickBottom"
        />
        <path
          d="m47.365 203.93 13.863-13.863v-89.628l-13.863-13.863z"
          stroke-width="2.6458"
          :fill="dienteLeft == '0' ? '#ffffff' : dienteLeft == '1' ? '#fba5a4' : '#92c5fc'"
          @click="clickLeft"
        />
      </g>
    </svg>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    top: Number,
    right: Number,
    bottom: Number,
    left: Number,
    center: Number
  },
  data () {
    return {
      dienteTop: this.top,
      dienteRight: this.right,
      dienteBottom: this.bottom,
      dienteLeft: this.left,
      dienteCenter: this.center
    }
  },
  mounted () {
    console.log("csaca")
  },
  methods: {
    clickCenter () {
      if (this.dienteCenter === 0) {
        this.dienteCenter = 1
      } else {
        if (this.dienteCenter === 1) {
          this.dienteCenter = 2
        } else {
          this.dienteCenter = 0
        }
      }
    },
    clickTop () {
      if (this.dienteTop === 0) {
        this.dienteTop = 1
      } else {
        if (this.dienteTop === 1) {
          this.dienteTop = 2
        } else {
          this.dienteTop = 0
        }
      }
    },
    clickRight () {
      if (this.dienteRight === 0) {
        this.dienteRight = 1
      } else {
        if (this.dienteRight === 1) {
          this.dienteRight = 2
        } else {
          this.dienteRight = 0
        }
      }
    },
    clickBottom () {
      if (this.dienteBottom === 0) {
        this.dienteBottom = 1
      } else {
        if (this.dienteBottom === 1) {
          this.dienteBottom = 2
        } else {
          this.dienteBottom = 0
        }
      }
    },
    clickLeft () {
      if (this.dienteLeft === 0) {
        this.dienteLeft = 1
      } else {
        if (this.dienteLeft === 1) {
          this.dienteLeft = 2
        } else {
          this.dienteLeft = 0
        }
      }
    },
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
