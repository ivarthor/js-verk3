1) þegar það er gert breytu sem bendir til object þá bendir breytan bara til objectin en breytist aldrei í það
með breytur þá breytast breyturnar í breytuna sem er bent á

2) fyrst er gert fallið Book sem er constructor síðan er gert aðferð fyrir fallið sem heitir getIsbn með Book.prototype.getIsbn síðan er búið til object sem kallar á fallið sem keyrir aðferðina á fallinu.

3) 
function Flaug(speed, lif) {
      this.speed = speed;
      this.lif = lif;
}

Flaug.prototype.fly = function () {
    this.speed += 1;
}

let f1 = new Flaug(1,10);
let f2 = new Flaug(2,10);
let f3 = new Flaug(3,10);

f1.setLife = function () {
    this.lif += 1;
};

4)
class Flaugar {
    constructor(speed, lif) {
        this.speed = speed;
        this.lif = lif;
    }
    
    fly() {
       this.speed += 1; 
    }
}

let f1 = new Flaug(1,10);
let f2 = new Flaug(2,10);
let f3 = new Flaug(3,10);

f1.setLife = function () {
    this.lif += 1;
};

5) class er tæknilega ekki til í javascript það er bara í sumum tilfellum þæginlegri að nota og léttara að skilja en bakvið tjöldin mun prototype vera í stjórn.
