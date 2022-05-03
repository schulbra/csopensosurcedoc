<h1 align="center">SpaceX REST API</h1>
<p align="center"><img src="https://live.staticflickr.com/65535/49185149122_37f5c52e43_k.jpg"></p>


<p align="LEFT">
 <table id="tableForm2">
 <thead>
 <tr>
  <th></th>
 </tr>
 
 <tr>
  <td><label for="medID"><a href="https://hub.docker.com/r/jakewmeyer/spacex-api/"><img src="https://img.shields.io/docker/pulls/jakewmeyer/spacex-api?style=flat-square"></a></label></td>
  <td><label for="id"><a href="https://github.com/r-spacex/SpaceX-API/actions?query=workflow%3ATest"><img src="https://img.shields.io/github/workflow/status/r-spacex/SpaceX-API/Test?style=flat-square"></a></label></td>
  <td><label for="medID"><a href="https://github.com/r-spacex/SpaceX-API/releases"><img src="https://img.shields.io/github/release/r-spacex/SpaceX-API.svg?longCache=true&style=flat-square"></a></label></td>
  <td><label for="medID"><a href="https://en.wikipedia.org/wiki/Representational_state_transfer"><img src="https://img.shields.io/badge/interface-REST-brightgreen.svg?longCache=true&style=flat-square"></a></label></td>
 </tr>

 <tr>
  <td><label for="medID"><a href="docs/README.md">Docs</a></label></td>
  <td><label for="id"><a href="docs/clients.md">API Clients</a></label></td>
  <td><label for="medID"><a href="docs/apps.md">Apps</a></label></td>
  <td><label for="medID"> <a href="https://status.spacexdata.com">Status</a></a></label></td>
 </tr>

 </thead>
 </table>










</p>



<h3 align="LEFT">
Project is:
</h3>

<h4 align="LEFT">
<i>
  An Open Source REST API for launch, rocket, core, capsule, starlink, launchpad, and landing pad data.
  </i>
</h4>

<h3 align="LEFT">
Project is NOT:
</h3>
<h4 align="LEFT">
  <i>
    Affiliated, associated, authorized, endorsed by, or in any way officially connected with Space Exploration Technologies Corp (SpaceX), or any of its subsidiaries or its affiliates. The names SpaceX as well as related names, marks, emblems and images are registered trademarks of their respective owners.
  </i>
</h4>


<h3 align="LEFT">
How To Use:
</h3>
<h4 align="LEFT">
 <p><b><i> **Already know what an API is? Skip to Usage below! </b></p></i>
 <p><b> Whats an API and how do I make sense of any of this? </b></p>
 <p><b> API is an abbreviation for Application Programming Interface which is a collection of communication protocols and subroutines used by various programs to communicate between them. A programmer can make use of various API tools to make its program easier and simpler. Also, an API facilitates the programmers with an efficient way to develop their software programs.
 Thus in simpler terms, an API helps two programs or applications to communicate with each other by providing them with necessary tools and functions. It takes the request from the user and sends it to the service provider and then again sends the result generated from the service provider to the desired user.
 </b></p>

 <b><p> A developer extensively uses API’s in his software to implement various features by using an API call without writing the complex codes for the same. We can create an API for an operating system, database systems, hardware system, for a JavaScript file or similar object oriented files. Also, an API is similar to a GUI(Graphical User Interface) with one major difference. Unlike GUI’s, an API helps the software developers to access the web tools while a GUI helps to make a program easier to understand by the users. (AkshitaKumawat, 2018)
</b></p>

<p><b>
 This project is a REST API, which in simple terms is a means for allowing you to access various records
 related to SpaceX.
</b></p>

<form id="showTable">
             <table id="tableForm2">
               <thead>
                <tr>
                  <th>Example:</th>
                  <th></th>
                  <th></th>
                </tr>
                <tr>
                 <td><label for="id"><b>____________________</b></label></td>
                </tr>
                <tr>
                 <td><label for="id"><b>GET One Capsule:</b></label></td>
                                   <td> =| </td>
                 <td><label for="id">Obtain all data on one specified capsule</label></td>
                </tr>
                <tr>
                 <td><label for="disease"> Outline of Comnmand   </label></td>
                  <td> =| </td>
                 <td><label for="id">https://api.spacexdata.com/v3/capsules/{{capsule_serial}}</label></td>
                </tr>
                <tr>
                   <td><label for="disease">                 capsule_serial   </label></td>
                   <td> =| </td>
                   <td><label for="disease">capsules serial id #</label></td>
                </tr>
                <tr>
                   <td><label for="disease">           sample capsule ID   </label></td>
                                      <td> =| </td>
                   <td><label for="disease">c112 </label></td>
                </tr>
                <tr>
                   <td><label for="disease">                        Variable type   </label></td>
                                      <td> =| </td>
                   <td><label for="disease">String</label></td>
                </tr>
                                <tr>
                 <td><label for="id"><b>____________________</b></label></td>
                </tr>
                <tr>
                     <td><label for="id"><b>Command/Request:</b></label></td>
                     <td> =| </td>
                     <td><label for="id">  curl --location --request GET 'https://api.spacexdata.com/v3/capsules/C112 </label></td>
                </tr>
                                <tr>
                 <td><label for="id"><b>____________________</b></label></td>
                </tr>
                <tr>
                     <td><label for="id"><b>Command/Response:</b></label></td>
                </tr>
                <tr><td>{</td> </tr>
                <tr><td> " capsule_serial": "C112",</td> </tr>
                 <tr><td>" capsule_id": "dragon1",</td> </tr>
                 <tr><td>" status": "active",</td> </tr>
                 <tr><td>" original_launch": "2017-02-19T14:39:00.000Z",</td> </tr>
                 <tr><td>" original_launch_unix": 1487515140,</td> </tr>
                <tr><td> " missions": [</td> </tr>
                <tr><td>  {</td> </tr>
                  <tr><td>   " name": "CRS-10",</td> </tr>
                <tr><td>      " flight": 36</td> </tr>
                 <tr><td>}</td> </tr>
                <tr><td> ],</td> </tr>
                <tr><td>" landings": 1,</td> </tr>
                <tr><td>" type": "Dragon 1.1",</td> </tr>
                <tr><td>" details": null,</td> </tr>
                <tr><td>" reuse_count": 0</td> </tr>
                <tr>
                                <tr>
                 <td><label for="id"><b>____________________</b></label></td>
                </tr>
                <td><label for="medID"><a href="https://www.geeksforgeeks.org/introduction-to-apis/">Learn More About APIS Here</a></label></td>
                </tr>
  </thead>
 </table> 
</h4>
<form id="showTable">




## Usage

```http
GET https://api.spacexdata.com/v4/launches/latest
```

```json
{
  "fairings": null,
  "links": {
    "patch": {
      "small": "https://images2.imgbox.com/eb/0f/Vev7xkUX_o.png",
      "large": "https://images2.imgbox.com/ab/79/Wyc9K7fv_o.png"
    },
    "reddit": {
      "campaign": "https://www.reddit.com/r/spacex/comments/fjf6rr/dm2_launch_campaign_thread/",
      "launch": "https://www.reddit.com/r/spacex/comments/glwz6n/rspacex_cctcap_demonstration_mission_2_general",
      "media": "https://www.reddit.com/r/spacex/comments/gp1gf5/rspacex_dm2_media_thread_photographer_contest/",
      "recovery": "https://www.reddit.com/r/spacex/comments/gu5gkd/cctcap_demonstration_mission_2_stage_1_recovery/"
    },
    "flickr": {
      "small": [],
      "original": [
        "https://live.staticflickr.com/65535/49927519643_b43c6d4c44_o.jpg",
        "https://live.staticflickr.com/65535/49927519588_8a39a3994f_o.jpg",
        "https://live.staticflickr.com/65535/49928343022_6fb33cbd9c_o.jpg",
        "https://live.staticflickr.com/65535/49934168858_cacb00d790_o.jpg",
        "https://live.staticflickr.com/65535/49934682271_fd6a31becc_o.jpg",
        "https://live.staticflickr.com/65535/49956109906_f88d815772_o.jpg",
        "https://live.staticflickr.com/65535/49956109706_cffa847208_o.jpg",
        "https://live.staticflickr.com/65535/49956109671_859b323ede_o.jpg",
        "https://live.staticflickr.com/65535/49955609618_4cca01d581_o.jpg",
        "https://live.staticflickr.com/65535/49956396622_975c116b71_o.jpg",
        "https://live.staticflickr.com/65535/49955609378_9b77e5c771_o.jpg",
        "https://live.staticflickr.com/65535/49956396262_ef41c1d9b0_o.jpg"
      ]
    },
    "presskit": "https://www.nasa.gov/sites/default/files/atoms/files/commercialcrew_press_kit.pdf",
    "webcast": "https://youtu.be/xY96v0OIcK4",
    "youtube_id": "xY96v0OIcK4",
    "article": "https://spaceflightnow.com/2020/05/30/nasa-astronauts-launch-from-us-soil-for-first-time-in-nine-years/",
    "wikipedia": "https://en.wikipedia.org/wiki/Crew_Dragon_Demo-2"
  },
  "static_fire_date_utc": "2020-05-22T17:39:00.000Z",
  "static_fire_date_unix": 1590169140,
  "tdb": false,
  "net": false,
  "window": 0,
  "rocket": "5e9d0d95eda69973a809d1ec",
  "success": true,
  "failures": [],
  "details": "SpaceX will launch the second demonstration mission of its Crew Dragon vehicle as part of NASA's Commercial Crew Transportation Capability Program (CCtCap), carrying two NASA astronauts to the International Space Station. Barring unexpected developments, this mission will be the first crewed flight to launch from the United States since the end of the Space Shuttle program in 2011. DM-2 demonstrates the Falcon 9 and Crew Dragon's ability to safely transport crew to the space station and back to Earth and it is the last major milestone for certification of Crew Dragon. Initially the mission duration was planned to be no longer than two weeks, however NASA has been considering an extension to as much as six weeks or three months. The astronauts have been undergoing additional training for the possible longer mission.",
  "crew": [
    "5ebf1b7323a9a60006e03a7b",
    "5ebf1a6e23a9a60006e03a7a"
  ],
  "ships": [
    "5ea6ed30080df4000697c913",
    "5ea6ed2f080df4000697c90b",
    "5ea6ed2f080df4000697c90c",
    "5ea6ed2e080df4000697c909",
    "5ea6ed2f080df4000697c90d"
  ],
  "capsules": [
    "5e9e2c5df359188aba3b2676"
  ],
  "payloads": [
    "5eb0e4d1b6c3bb0006eeb257"
  ],
  "launchpad": "5e9e4502f509094188566f88",
  "auto_update": true,
  "flight_number": 94,
  "name": "CCtCap Demo Mission 2",
  "date_utc": "2020-05-30T19:22:00.000Z",
  "date_unix": 1590866520,
  "date_local": "2020-05-30T15:22:00-04:00",
  "date_precision": "hour",
  "upcoming": false,
  "cores": [
    {
      "core": "5e9e28a7f3591817f23b2663",
      "flight": 1,
      "gridfins": true,
      "legs": true,
      "reused": false,
      "landing_attempt": true,
      "landing_success": true,
      "landing_type": "ASDS",
      "landpad": "5e9e3032383ecb6bb234e7ca"
    }
  ],
  "id": "5eb87d46ffd86e000604b388"
}
```

## Cron Job Status

<p align="left">
<img src="https://healthchecks.io/badge/a99e6369-9795-417e-9a1c-31ea91/zDDqPvw1-2/Capsules.svg">
<br/>
<img src="https://healthchecks.io/badge/a99e6369-9795-417e-9a1c-31ea91/iJIWcg9u-2/Cores.svg">
<br/>
<img src="https://healthchecks.io/badge/a99e6369-9795-417e-9a1c-31ea91/soA1Z2t1-2/Landpads.svg">
<br/>
<img src="https://healthchecks.io/badge/a99e6369-9795-417e-9a1c-31ea91/tc7aK4Iw-2/Launchpads.svg">
<br/>
<img src="https://healthchecks.io/badge/a99e6369-9795-417e-9a1c-31ea91/uB7PIyUo-2/Past-Launches.svg">
<br/>
<img src="https://healthchecks.io/badge/a99e6369-9795-417e-9a1c-31ea91/bQw1ZrmZ-2/Payloads.svg">
<br/>
<img src="https://healthchecks.io/badge/a99e6369-9795-417e-9a1c-31ea91/HhIoHcF6-2/Roadster.svg">
<br/>
<img src="https://healthchecks.io/badge/a99e6369-9795-417e-9a1c-31ea91/wPz7gFQJ-2/Starlink.svg">
<br/>
<img src="https://healthchecks.io/badge/a99e6369-9795-417e-9a1c-31ea91/3L5HxZKX-2/Upcoming-Launches.svg">
<br/>
<img src="https://healthchecks.io/badge/a99e6369-9795-417e-9a1c-31ea91/YvnZYkED-2/Webcast.svg">
<br/>
<img src="https://healthchecks.io/badge/a99e6369-9795-417e-9a1c-31ea91/_Z-lNpev-2/launch-library-v2.svg">
</p>

## Sponsors

### [Studio 3T](https://studio3t.com/)

[![Studio 3T](https://imgur.com/DbJSfAo.png)](https://studio3t.com/)

## FAQ's

* If you have any questions or corrections, please open an issue and we'll get it merged ASAP
* For any other questions or concerns, just shoot me an email.
