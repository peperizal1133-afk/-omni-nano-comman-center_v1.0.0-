# -omni-nano-comman-center_v1.0.0-
THE TIME ENGINE OF THE TWINOMNI.Time = {  speed: 1, // 1x real-time  start() {    setInterval(() => {      OMNI.Bus.emit("tick", {        timestamp: Date.now()      });    }, 1000 / this.speed);  },  accelerate(factor) {    this.speed = factor;  }};
