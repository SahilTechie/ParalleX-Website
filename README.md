# ParalleX-Website
This is First Project using HTML and CSS ....

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ParallelX Website</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div id="wrapper">
        <div class="container">
            <img src="background.png" class="background">
            <img src="foreground.png" class="foreground">
            <h1>ADVENTURE</h1>
        </div>
        <section>
            <h2 class="secondheading">ADVENTURE TIME</h2>
            <p class="text"> 
                Adventure Time is an animated series that follows the adventures of Finn, a young boy, and his magical dog, Jake, in the Land of Ooo. Filled with quirky characters, surreal landscapes, and whimsical storylines, the show blends humor, emotion, and fantasy. Its unique art style, rich lore, and underlying themes of friendship, courage, and self-discovery have made it a beloved series for both children and adults alike.
                <br><br>
                Adventure Time is a fantastical animated series set in the post-apocalyptic Land of Ooo, where Finn, a brave human, and his magical dog companion, Jake, go on thrilling, often bizarre quests. The show’s colorful world is filled with eccentric characters like Princess Bubblegum, the Ice King, and Marceline the Vampire Queen, each with their own rich backstories. Its imaginative storytelling, blending adventure, humor, and deep emotional arcs, captures themes of love, change, and self-discovery, making it both whimsical and thought-provoking for audiences of all ages.
            </p>
            <div class="bg bg1">
                <h2 class="desc">BIKING</h2>
            </div>
            <p class="text"> 
                Biking is a versatile and enjoyable activity that combines exercise, transportation, and adventure. Whether cycling through city streets, rural paths, or rugged mountain trails, biking offers a unique sense of freedom and connection with the environment. It’s a low-impact exercise that enhances cardiovascular health, builds muscle strength, and improves overall stamina. For commuters, biking is an eco-friendly alternative to driving, reducing carbon emissions and contributing to cleaner air.
                <br><br>
                Beyond the physical benefits, biking can be a mentally refreshing experience. It allows for moments of reflection and relaxation, offering a break from the hustle of daily life. Many cyclists find joy in discovering new routes, challenging themselves on tough terrains, or simply enjoying the beauty of nature.

Biking also fosters a sense of community through cycling clubs, group rides, and events like charity rides or races. Whether done for sport, leisure, or as a sustainable way to travel, biking is a rewarding activity that promotes health, well-being, and environmental consciousness.
            </p>   
            <div class="bg bg2">
                <h2 class="desc">PARA GLINDING</h2>
            </div>
            <p class="text"> 
                Paragliding is an exhilarating adventure sport that involves flying lightweight, foot-launched gliders without any rigid primary structure. The pilot sits in a harness suspended below a fabric wing, which has a series of interconnected cells that allow the wing to inflate with air, creating lift. Unlike powered aircraft, paragliders rely solely on wind currents, thermals (rising warm air), and the pilot's navigation skills to stay airborne and move through the sky.
                <br><br>
                The sport offers a unique experience of flight, giving participants the sensation of soaring like a bird while enjoying breathtaking views from above. It can be done recreationally for sightseeing, or competitively, where pilots aim to cover long distances or perform precise maneuvers. Paragliding is often practiced in mountainous regions or coastal areas with favorable wind conditions, making it popular in locations like the Swiss Alps, the Himalayas, and coastal regions of Europe and South America.

Safety precautions are essential, as weather conditions and proper equipment play a critical role in ensuring a safe and enjoyable flight.
            </p>   
            <div class="bg bg3">
                <h2 class="desc">SURFING</h2>
            </div>
            <p class="text"> 
                Surfing is a water sport that involves riding on the face of a moving wave, typically using a surfboard. It originated in ancient Polynesia, with early records showing that it was an essential part of their culture, particularly in Hawaii, where it was considered the "sport of kings." In surfing, the rider paddles out to the wave, catches it, and uses the momentum of the wave to ride toward the shore while performing various maneuvers.
                <br><br>
                Modern surfing has evolved into a popular global sport with different styles, including longboarding, shortboarding, and big wave surfing, where surfers tackle enormous waves reaching up to 100 feet. Surfers develop skills in balance, timing, and wave reading, often seeking out the perfect wave in renowned surf spots like Hawaii, California, and Australia. Beyond just a sport, surfing is also viewed as a lifestyle, embodying a deep connection with nature, freedom, and the thrill of riding waves. Many surfers describe it as an almost meditative experience, blending physical skill with mental focus.
            </p>  
            <h2 class="myname">"SahilTechie.."</h2>
        </section>
    </div>
</body>
</html>


CSS CODE START FROM HERE :-

*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

#wrapper{
    height: 100vh;
    overflow-x: hidden;
    overflow-y: auto;
    perspective: 10px;
}

.container{
    position: relative;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    transform-style: preserve-3d;
    z-index: -1;
}

.background, .foreground{
     position: absolute;
     height: 100%;
     width: 100%; 
     object-fit: cover;
     z-index: -1;
}

.background{
    transform: translateZ(-40px) scale(6);
}

.foreground{
    transform: translateZ(-20px) scale(3);
}

h1{
    position: absolute;
    top: 7.5rem;
    font-size: 5rem;
    letter-spacing: 4px;
    color: whitesmoke;
    text-shadow: 0 0 10px rgba(0,0,0,0.3);
    font-family: Arial, Helvetica, sans-serif;
}

section{
    background-color: rgb(45,45,45);
    color: white;
    padding: 5rem 0;
}

.secondheading{
    font-size:3rem;
    padding: 0 4.5rem;
}

.text{
    font-size: 1.2rem;
    padding: 0 4em;
    margin: 5rem 0;
}

.bg1{
    background-image: url(sport-1.jpg);
}

.bg2{
    background-image: url(sport-2.jpg);
}

.bg3{
    background-image: url(sport-3.jpg);
}

.bg{
    position: relative;
    width: 100%;
    background-attachment: fixed;
    background-size: cover;
    background-position: center;
    height: 400px;
}

.desc{
    position: absolute;
    background-color: whitesmoke;
    color: black;
    padding: 0.5rem 2.5rem;
    top: 50%;
    left: 50%;
    transform: translateX(-50%) translateY(-50%);
    font-size: 2rem;
    font-weight: 600;
}

.myname{
    font-family: Arial, Helvetica, sans-serif;
    font-size:2rem;
    display: flex;
    justify-content: center; 
    align-items: center;    
    height: 100vh;   
}
