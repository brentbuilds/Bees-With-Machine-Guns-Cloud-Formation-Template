Bees-With-Machine-Guns-Cloud-Formation-Template
===============================================

This CloudFormation template is for users who want to autorun Bees with Machine Guns.  The issue with other templates is that the "bees" instances weren't ready when the controller wascalling the attack.  This results in the "your bees are peace loving hippies message".  To overcome this issue, "sleep 300 \n" was added to the create-swarm command.  

By adding the sleep command to the create-swarm command, it allows the instances a chance to initialize before being called by the controller.

Bees with Machine Guns AWS CloudFormation Template 
