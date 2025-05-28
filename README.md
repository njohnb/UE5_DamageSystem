# UE5_DamageSystem
A health and damage system for Unreal Engine 5 with varying damage types and effects.

#HOW TO USE
Add the BP_HealthComponent on to any actor.
In your actors Class Settings, add an Implemented Interface and select BPI_Damagable.
Now you can implement the apply damage event. (see BP_TestTarget for example usage) 
simple example. Call BP_HealthComponent's ApplyDamage and pass it DamageContext
NOTE: BPI_Damagable's ApplyDamage uses the custom BP_DamageContext struct
BP_DamageContext
	- Damage Amount
	- Damage type
	- Instigator
	- bIsCriticalHit