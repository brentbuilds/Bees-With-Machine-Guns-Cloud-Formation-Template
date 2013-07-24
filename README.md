Bees-With-Machine-Guns-Cloud-Formation-Template
===============================================

If you're getting the "Your bees are peace loving hippies" or other timeout errors, it is possible that your "bee" instances aren't initializing before they're called.

This CloudFormation template is for users who want to autorun Bees with Machine Guns.  The issue with other templates is that the "bees" instances weren't ready when the controller called the attack.  This would result in the following error message, "your bees are peace loving hippies" or other timeout errors.  To overcome this issue, "sleep 300 \n" was added to the create-swarm command.  

By adding the sleep command to the create-swarm command, it allows the instances a chance to initialize before being called by the controller.

Bees with Machine Guns AWS CloudFormation Template 
