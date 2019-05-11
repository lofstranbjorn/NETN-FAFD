---
title: 'Entity Tasking and Reporting (new)'
media_order: chairs-clock-desks-950098.jpg
date: '04-06-2018 12:15'
body_classes: 'header-transparent header-dark'
visible: true
hero_classes: 'text-light parrallax title-h1h2 overlay-dark'
hero_image: chairs-clock-desks-950098.jpg
blog_url: /blog
show_sidebar: false
show_breadcrumbs: false
show_pagination: false
continue_link: true
content:
    items: '@self.children'
    limit: '5'
    order:
        by: date
        dir: desc
    pagination: '1'
    url_taxonomy_filters: '1'
---

The **Low-Level Battle Management Language (LBML)**  is a part of the NETN SimC2 component and represent lower-level tasks suitable for providing simulation instructions to federates modelling individual units or platforms. 

LBML provides a simulator independent way of command and control over simulated entities both from a simulator operator perspective and when modelling command and control interaction between federates in a distributed simulation. LBML contains common low level tasks and commands that can easily be interpreted and executed by simulations that model the behavior of entities. It also defines a set of reports used by simulations to provide status updates of the tasks being executed. 

<table class="table">
  <thead>
    <tr>
      <th>Instructions</th>
      <th>Reports</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td valign="top">
<b>ChangeOrderedAltitude</b>: Request new altitude.</br>
<b>ChangeOrderedSpeed</b>: Request new speed.</br>
<b>FireAtLocation</b>: Task entity to fire at a location.</br>
<b>FireIndirectWM</b>: Task entity to fire at a location with the specified weapon and munition.</br>
<b>FireAtUnit</b>: Task entity to fire at a specified unit.</br>
<b>FireDirectWM</b>: Task entity to fire at a specified unit with specified weapon munition type.</br>
<b>FollowRoute</b>: Task entity to follow a specified route.</br>
<b>FollowUnit</b>: Tasks entity to follow another unit.</br>
<b>Move</b>: Task entity to move in the specified direction.</br>
<b>MoveIntoFormation</b>: Task an aggregate unit to move into specified formation and heading.</br>
<b>MoveToLocation</b>: Task unit to move to the specified destination.</br>
<b>MoveToUnit</b>: Task entity to move to another unit.</br>
<b>SetRulesOfEngagement</b>: Task a unit to change the rules of engagement.</br>
<b>TurnToHeading</b>: Task entity to turn to the specified heading.</br>
<b>TurnToOrientation</b>: Task entity to rotate to the specified orientation using pitch and roll parameters.</br>
<b>VehicleDismount</b>: Task entity to dismount from a vehicle.</br>
<b>VehicleMount</b>: Task entity to mount a specified vehicle.</br>
<b>Wait</b>: Tasks entity to wait until the specified end time.</br>
<b>CancelAllTasks</b>: Cancel all tasks. Tasks already started are aborted immediately. </br>
<b>CancelSpecifiedTasks</b>: Cancel all specified tasks. Tasks already started are aborted immediately.</br>
</td>
<td valign="top">
 <b>CurrentActivityStatusReport</b>: Report time and status of current task.</br>
<b>NextActivityStatusReport</b>: Report time and start condition of next activity.</br>
<b>AmmunitionStatusReport</b>: Report current amount of ammunition.</br>
<b>DamageStatusReport</b>: Report when damage state changes.</br>
<b>FuelStatusReport</b>: Report current amount of fuel left.</br>
<b>PositionStatusReport</b>: Report position, speed, and heading of simulated entity.</br>
<b>UnderAttackStatusReport</b>: Report when unit is under attack.</br>
<b>SpotReport</b>: Report when unit's sensors detect opposing, neutral, or unknown unit.</br>
<b>ActivitySpotReport</b>: Report the perceived current activity of a spotted unit.</br>
<b>CurrentActivitySpotReport</b>: Report elapsed time and status of the current task.</br>
<b>NextActivitySpotReport</b>: Report time and start condition of the next activity.</br>
<b>InSensorReport</b>: Report sensor type and identifiers of detected entities.</br>
<b>InWeaponRangeReport</b>: Report weapon type and identifiers of entities within weapon range. </br>
</td>
    
  </tbody>
</table>
<p/>