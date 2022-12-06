
# Wheel Module

## Description

This module is used for the Wheel part.

## Implementations

| Name                     | Description                                                                                | 
| ------------------------ | ------------------------------------------------------------------------------------------ | 
| [INJ_TurnAxisWheels](../world/Rocket.html#interfaces) | It is used to know where the player is turning.                                            | 
| [INJ_Physics](../world/Rocket.html#interfaces)        | To get the rocket [Rigibody 2D](https://docs.unity3d.com/ScriptReference/Rigidbody2D.html) | 
| [I_PartMenu](../world/Rocket.html#interfaces)         | This allow draw wheel statistics in Build screen                                           | 

## Properties

| Type                 | Name               | Description                      | 
| -------------------- | ------------------ | -------------------------------- | 
| [Bool_Reference](../variables/BoolReference.html) | on                 | Store if the wheel is on         | 
| float                | angularVelocity    | Get the current angular velocity | 
| float                | maxAngularVelocity | Get the max angular velocity     | 
| float                | traction           | Wheel traction                   | 
| float                | power              | Wheel power                      | 

## Public Methods

| Type | Name          | Description              | 
| ---- | ------------- | ------------------------ | 
| void | ToggleEnabled | Turn On or OFF the wheel | 

## Private Methods

| Type | Name              | Description                                                                                                                              | 
| ---- | ----------------- | ---------------------------------------------------------------------------------------------------------------------------------------- | 
| void | OnCollisionStay2D | This function is executed when the wheel touches a surface with [Collider 2D](https://docs.unity3d.com/ScriptReference/Collider2D.html). | 
| void | Update            | Here the rotation animation is applied taking into account the angular velocity                                                          | 

