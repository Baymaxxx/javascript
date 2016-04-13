Math.abs(5)   // 5
Math.abs(-5)  // 5

Math.round(1.1)   // 1
Math.round(1.9)   // 2

Math.ceil(1.1)   // 2
Math.ceil(1.9)   // 2

Math.floor(1.1)   // 1
Math.floor(1.9)   // 1

Math.max(1,2)      // 2
Math.max(-1,-2,-3) // -1

Math.min(1,2)      // 1
Math.min(-1,-2,-3) // -3

Math.random()  // 大于等于0且小于1的随机数

parseInt('1.1')    // 1
parseInt('1.9')    // 1
parseInt('1b2.4')  // 1
parseInt('www')    // NaN

parseFloat('100.1')  // 100.1
parseFloat('12.4b5') // 12.4
parseFloat('www')    // NaN

Number('100.1')    // 100.1
Number('12.4b5')   // NaN
Number('www')      // NaN

(100.123).toFixed(2)   //  "100.12"
(100.123).toFixed(0)   //  "100"
