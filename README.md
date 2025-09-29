# lecture-9
JavaScript: new Date, new Set, and new Map
Introduction

Дар ин ҳуҷҷат, мо ба се мавзуи асосӣ дар JavaScript, ки дар ҷаҳони барномасозӣ маъруфанд, назар хоҳем андохт:

new Date

new Set

new Map

1. new Date()

Дар JavaScript, Date() барои кор кардани бо сана ва вақт истифода мешавад. Шумо метавонед объекти санаи шенасоиро бо усулҳои зиёд истифода кунед.

Методҳои "get"

Методҳои "get" барои гирифта шудани маълумот дар бораи сана истифода мешаванд. Масалан:

getFullYear() - Маъзарат, солро ҳамчун рақам гирифта мекунад.

getMonth() - Моҳро (0 то 11) гирифта мекунад.

getDate() - Рӯзро (1 то 31) гирифта мекунад.

getHours() - Соатро (0 то 23) гирифта мекунад.

Масал:

let currentDate = new Date();
console.log(currentDate.getFullYear());  // 2025
console.log(currentDate.getMonth());     // 8 (Сентябр)

Методҳои "set"

Методҳои "set" барои таъйин кардани сана, соат ё дигар ҷузъиёти сана истифода мешаванд:

setDate() - Рӯзи моҳро таъйин мекунад.

setMonth() - Моҳро таъйин мекунад.

setFullYear() - Соли санаи хосро таъйин мекунад.

Масал:

let newDate = new Date();
newDate.setFullYear(2023);
newDate.setMonth(4);  // Моҳи май
console.log(newDate);

2. new Set()

Set як объекти махсус аст, ки фақат унсурҳои беназири худро нигоҳ медорад. Агар шумо як унсури дубора ворид кунед, он автоматикӣ қатъ карда мешавад.

Масал:
let mySet = new Set();
mySet.add(1);
mySet.add(2);
mySet.add(2);  // 2 дубора ворид намешавад
console.log(mySet);  // Set { 1, 2 }


Методи has() барои тафтиши аъзои Set.

delete() барои ҳазфи аъзои Set.

3. new Map()

Map объектест, ки ба шумо имкон медиҳад, ки калид ва арзишҳоро захира кунед. Бар unlike "Set", Map кӯмак мекунад, ки ҳар як калид дорои арзиш бошад.

Масал:
let myMap = new Map();
myMap.set('name', 'Alice');
myMap.set('age', 25);
console.log(myMap.get('name'));  // Alice


Методи set() барои таъйин кардани калид ва арзиш.

get() барои гирифтани арзиш тавассути калид.