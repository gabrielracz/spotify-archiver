# spotify-archiver
Create ascii tables for public spotify playlsts. \
Live demo at [https://gsracz.com/spotify-archiver.html](https://gsracz.com/spotify-archiver.html)

## Instructions
- Have Node.js installed
- Get your [Spotify API client-secret and client-id](https://developer.spotify.com/documentation/web-api/tutorials/getting-started#create-an-app)
and place them in corresponding ```.client-secret``` and ```.client-id``` files in the spotify-archiver.js directory.
- Run with target username, playlist name, and options:

        $ node spotify-archiver.js gabriel.racz rock [options]
### Options
- ```--list``` - list all public playlists for given username
        
        $ node spotify-archiver.js gabriel.racz --list
        
- ```--albums``` - include album names in the table

        $ node spotify-archiver.js gabriel.racz classics --albums
        
## Examples
- Simple

        $ node spotify-archiver.js gabriel.racz metal
        +----------------------------------------------------------------+---------------------+
        | Track                                                          | Artist              | 
        +----------------------------------------------------------------+---------------------+
        | Sabbath Bloody Sabbath - 2014 Remaster                         | Black Sabbath       | 
        | Snowblind - 2014 Remaster                                      | Black Sabbath       | 
        | Hand of Doom - 2012 - Remaster                                 | Black Sabbath       | 
        | The Trooper - 2015 Remaster                                    | Iron Maiden         | 
        | Planet Caravan - 2012 - Remaster                               | Black Sabbath       | 
        | Solitude - 2014 Remaster                                       | Black Sabbath       | 
        | Under the Sun - 2014 Remaster                                  | Black Sabbath       | 
        | Paranoid - 2012 - Remaster                                     | Black Sabbath       | 
        | Supernaut - 2014 Remaster                                      | Black Sabbath       | 
        | N.I.B.                                                         | Black Sabbath       | 
        | A Bit of Finger / Sleeping Village / Warning - 2013 Remaster   | Black Sabbath       | 
        | Megalomania - 2013 Remaster                                    | Black Sabbath       | 
        | Wheels of Confusion / The Straightener - 2014 Remaster         | Black Sabbath       | 
        | Sweet Leaf - 2014 Remaster                                     | Black Sabbath       | 
        | Spiral Architect - 2013 Remaster                               | Black Sabbath       | 
        | Hole in the Sky - 2014 Remaster                                | Black Sabbath       | 
        | The Thrill of it All - 2013 Remaster                           | Black Sabbath       | 
        | Fade To Black (Remastered)                                     | Metallica           | 
        | Hallowed Be Thy Name - 2015 Remaster                           | Iron Maiden         | 
        | Nothing Else Matters                                           | Metallica           | 
        | The Day That Never Comes                                       | Metallica           | 
        | The Unforgiven                                                 | Metallica           | 
        | War Pigs                                                       | Black Sabbath       | 
        | Buried Alive                                                   | Avenged Sevenfold   | 
        | Wherever I May Roam                                            | Metallica           | 
        | To Live Is to Die (Remastered)                                 | Metallica           | 
        | Orion (Remastered)                                             | Metallica           | 
        | Welcome Home (Sanitarium) (Remastered)                         | Metallica           | 
        | Through the Fire and Flames                                    | DragonForce         | 
        | Master of Puppets (Remastered)                                 | Metallica           | 
        | Fear of the Dark - 2015 Remaster                               | Iron Maiden         | 
        | Wasting Love - 2015 Remaster                                   | Iron Maiden         | 
        | Revelations - 2015 Remaster                                    | Iron Maiden         | 
        | Prodigal Son - 2015 Remaster                                   | Iron Maiden         | 
        | Aces High - 2015 Remaster                                      | Iron Maiden         | 
        | Into the Void - 2014 Remaster                                  | Black Sabbath       | 
        | Prowler - 2015 Remaster                                        | Iron Maiden         | 
        | A National Acrobat - 2013 Remaster                             | Black Sabbath       | 
        | Sabbra Cadabra - 2013 Remaster                                 | Black Sabbath       | 
        | The Call Of Ktulu (Remastered)                                 | Metallica           | 
        | Red Tide Rising                                                | Orange Goblin       | 
        | The Wolf Bites Back                                            | Orange Goblin       | 
        | Bfg Division                                                   | Mick Gordon         | 
        | Apokatastasis Panton                                           | Deathspell Omega    | 
        | Initiation                                                     | Green Lung          | 
        | Electric Funeral - 2012 - Remaster                             | Black Sabbath       | 
        | The Stage                                                      | Avenged Sevenfold   | 
        | Coming Home                                                    | Avenged Sevenfold   | 
        | St. James                                                      | Avenged Sevenfold   | 
        +----------------------------------------------------------------+---------------------+
- List public playlists
        
        $ node spotify-archiver.js gabriel.racz --list
        +-------------------------------+
        | gabriel.racz's Playlists      |
        +-------------------------------+
        | master                        |
        | Fizică                        |
        | My Playlist #12               |
        | potential                     |
        | ambo                          |
        | metal                         |
        | tech                          |
        | razzman                       |
        | classics                      |
        | rock                          |
        | bang                          |
        | cinematic                     |
        +-------------------------------+

     
- Include albums

        $ node spotify-archiver.js gabriel.racz potential --albums
        +------------------------------------------------+--------------------------+-----------------------------------------------------------------------+
        | Track                                          | Artist                   | Album                                                                 |
        +------------------------------------------------+--------------------------+-----------------------------------------------------------------------+
        | Right Where It Belongs                         | Nine Inch Nails          | With Teeth                                                            |
        | Without Any Words (Only Crying and Laughter)   | '68                      | Two Parts Viper                                                       |
        | An Alternative to Freedom                      | Witchcraft               | Legend                                                                |
        | Where Devils Weep                              | Jonathan Hulten          | Chants from Another Place                                             |
        | A Dance in the Road                            | Jonathan Hulten          | Chants from Another Place                                             |
        | The Mountain                                   | Jonathan Hulten          | The Mountain                                                          |
        | Leaving                                        | Jonathan Hulten          | The Dark Night of the Soul                                            |
        | I Say Fever                                    | Ramona Falls             | Intuit                                                                |
        | Spore                                          | Ramona Falls             | Prophet                                                               |
        | Far Away                                       | Jose Gonzalez            | Far Away                                                              |
        | Malstroem                                      | Witchcraft               | Nucleus                                                               |
        | We: We Are Them                                | Siena Root               | Different Realities                                                   |
        |                                                | Nick Johnston            | ~~                                                                    |
        | Pull Away/So Many Times                        | Dust                     | Hard Attack/Dust                                                      |
        | Aphasia                                        | The Budos Band           | Burnt Offering                                                        |
        | Tide of Tears                                  | The Parlor Mob           | And You Were A Crow                                                   |
        | Pride                                          | Manchester Orchestra     | Mean Everything To Nothing                                            |
        | Remarkably Human                               | Nick Johnston            | Remarkably Human                                                      |
        | Can't Keep No Good Boy Down                    | The Parlor Mob           | And You Were A Crow                                                   |
        | Ben's My Friend                                | Sun Kil Moon             | Benji                                                                 |
        | Heron Blue                                     | Sun Kil Moon             | April                                                                 |
        | Shotgun                                        | Earl Greyhound           | Suspicious Package                                                    |
        | Fly...Night Bird                               | Roy Buchanan             | You're Not Alone                                                      |
        | Spring Break 1899                              | Murder By Death          | Red of Tooth and Claw                                                 |
        | Jules                                          | Seth Chapla              | Ascent                                                                |
        | Antechamber                                    | Latitudes                | Agonist                                                               |
        | Paradise Warfare                               | Carpenter Brut           | TRILOGY                                                               |
        | To You I Give                                  | Crippled Black Phoenix   | Great Escape                                                          |
        | Elk.Blood.Heart                                | All Them Witches         | Our Mother Electricity                                                |
        | Almost Was Good Enough                         | Magnolia Electric Co.    | Trials & Errors                                                       |
        | Whip-poor-will                                 | Magnolia Electric Co.    | Josephine                                                             |
        | Northstar Blues                                | Magnolia Electric Co.    | What Comes After The Blues                                            |
        | Autopilot                                      | Mondo Generator          | Demolition Day                                                        |
        | Time Go                                        | Caught A Ghost           | Human Nature                                                          |
        | Did You See Me?                                | Ween                     | Shinola (Vol. 1)                                                      |
        | Bronx Sniper                                   | Mister Heavenly          | Out of Love                                                           |
        | Autumn Leaves                                  | Burzum                   | The Ways of Yore                                                      |
        | Buckingham Green                               | Ween                     | The Mollusk                                                           |
        | I Fell In Love Today                           | Ween                     | Shinola (Vol. 1)                                                      |
        | Joker And The Thief                            | Wolfmother               | Wolfmother (10th Anniversary Deluxe Edition)                          |
        | Tuulee                                         | Mara Balls               | Elava kivi                                                            |
        | 0                                              | Omar Rodriguez-Lopez     | Omar Rodriguez-Lopez & John Frusciante                                |
        | Nimrodel / The Procession / The White Rider    | Camel                    | Mirage                                                                |
        | Shark Fin Blues                                | The Drones               | Wait Long By the River and the Bodies of Your Enemies Will Float By   |
        | Bus Stop Boxer                                 | Eels                     | Souljacker                                                            |
        | Mr. E's Beautiful Blues                        | Eels                     | Meet The EELS: Essential EELS 1996-2006 Vol. 1                        |
        | Love                                           | Colour Haze              | Colour Haze                                                           |
        +------------------------------------------------+--------------------------+-----------------------------------------------------------------------+
