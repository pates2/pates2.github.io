const inputDriver =  document.querySelector("[name='driver']");

  fetch(`https://www.simsprintseries.pl/api/driver`)
  .then(response => response.json())
      .then(data => data.sort((a,b) => (a.name > b.name) ? 1 : ((b.name > a.name) ? -1 : 0)).forEach(item => inputDriver.innerHTML += `<option value="${item.id}">${item.name}</option>`));

document.querySelectorAll(".input")
  .forEach(el => {
  el.addEventListener("change", () => call(inputDriver.value))
    });

const call = (driverId) => {
  fetch(`https://www.simsprintseries.pl/api/driver/${driverId}`)
  .then(response => response.json())
      .then(data => run(data, driverId));
}

const run = (d, driverId) =>  {
  const gp = [];
  const points = [];
  const positions = [];
  var dnfs = 0;
  var poles = 0;
  var fl = 0;
  d.results.forEach(result => {
      gp.push(`${result.race.relatedevent.name} ${result.race.name}`);
      points.push(result.points);
      positions.push(result.position)
      if(result.dnf === true){
        dnfs++;
      };
      if(result.pole === true){
        poles++;
      };
      if(result.fl === true){
        fl++;
      };
  });
  var allPoints = points.reduce(function(a, b){
        return a + b;
    }, 0);
  
  var allPositions = positions.reduce(function(a, b){
        return a + b;
    }, 0);
  
  var avgPoints = Math.round(allPoints/gp.length) || "Niedostępne";
  var avgPosition = Math.round(allPositions/gp.length) || "Niedostępne";
  var dnfProcent = Math.round((dnfs/gp.length)*100) || "0";
  
  document.getElementById("all-races").innerHTML = "Wyścigi: " + gp.length;
  document.getElementById("all-points").innerHTML = "Punkty: " + allPoints;
  document.getElementById("poles").innerHTML = "Pole position: " + dnfs;
  document.getElementById("fl").innerHTML = "Najszybsze okrążenia: " + dnfs;
  document.getElementById("dnf").innerHTML = "DNFy: " + dnfs;
  document.getElementById("points").innerHTML = "Średnia liczba punktów na wyścig: " + avgPoints;
  document.getElementById("position").innerHTML = "Średnia pozycja w wyścigu: " + avgPosition;
  document.getElementById("dnfs").innerHTML = "Nieukończone wyścigi: " + dnfProcent + "%" ;
};

