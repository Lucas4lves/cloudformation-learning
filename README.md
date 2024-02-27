# Learning Cloud Formation

 * A record of my developments on IaC with Cloud Formation


## Updating a Stack:

 * Depends on the attributes changed within a AWS resource:

   * WITH NO INTERRUPTION: does not change physical ID nor its service availability;
   * WITH SOME INTERRUPTION: does not change physical ID and blocks service availability for a while;
   * REPLACEMENT: changes physical ID (recreate resources from ground up);