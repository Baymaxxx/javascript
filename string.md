"micromajor".length  // 10

"micromajor".charAt(0)   // "m"
"micromajor".charAt(100) // ""

"micro-major".indexOf("-")     // 5
"micro-major-web".indexOf("-") // 5
"micro-major".indexOf("major") // 6
"micromajor".indexOf("-")      // -1

"micromajor163".search(/[0-9]/) // 10
"micromajor163".search(/[A-Z]/) // -1

"micromajor163".match(/[0-9]/) // ["1"]
"micromajor163".match(/[0-9]/g)// ["1","6","3"]
"micromajor163".match(/[A-Z]/) // null

"micromajor163".replace("163","###")  // "micromajor###"
"micromajor163".replace(/[0-9]/,"#")  // "micromajor#63"
"micromajor163".replace(/[0-9]/g,"#") // "micromajor###"
"micromajor163".replace(/[0-9]/g,"")  // "micromajor"

"micromajor".substring(5,7)  // "ma"
"micromajor".substring(5)    // "major"

"micromajor".slice(5,7)   // "ma"
"micromajor".slice(5)     // "major"
"micromajor".slice(1,-1)  // "icromajo"
"micromajor".slice(-3)    // "jor"

"micromajor".substr(5,2)  // "ma"
"micromajor".substr(5)    // "major"

"micro major".split(" ")     // ["micro","major"]
"micro major".split(" ",1)   // ["micro"]
"micro2major".split(/[0-9]/) // ["micro","major"]

"MicroMajor".toLowerCase()  // "micromajor"

"MicroMajor".toUpperCase()  // "MICROMAJOR"

"0571" + "-" + "88888888"  // "0571-88888888"

String(163)  // "163"
String(null) // "null"

"micro\"major"  // "micro"major"
"micro\\major"  // "micro\major"
"micro\tmajor"  // "micro	major"