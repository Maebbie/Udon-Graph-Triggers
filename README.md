## **Latest release: https://github.com/Maebbie/Udon-Graph-Triggers/releases**

**Udon Graph Triggers** contains an essential assortment of Triggers, ready to use for setting up basic world interactions in VRChat. It has both regular and synched variants.

Scroll down for a Quick Start Guide.

<img src="https://github.com/user-attachments/assets/6a05e8db-eacf-444a-9332-e670c2ac3c3f" width="426">

To use these, simply add a Udon Behaviour Script to a Game Object and drag the desired Behaviour into the "Program Source" field. All relevant options appear afterwards.

!! **Ensure that Synced Triggers ( those starting with " Sync_" ) have their Synchronization set to 'Manual' on the Udon Behaviour.** !!\
See the Quick Start Guide below.

Multiple Triggers can be used in the same Gameobject by adding Multiple Udon Behaviour Scripts to it.

<table border="0">
 <tr>
    <td><img src="https://github.com/Maebbie/Udon-Graph-Triggers/blob/main/Udon-Graph-Triggers_QuickStart.png" width="512"></td>
    <td><img src="https://github.com/Maebbie/Udon-Graph-Triggers/blob/main/Udon-Graph-Triggers-Listview.png" width="250"></td>
 </tr>
</table>

Found here are over 100 separate single purpose behaviours, that are loosely based on the old SDK2 trigger system's functionality.\
They follow a uniform Naming Convention:\
```Event Type - Affecting  - State```

For example:\
```OnInteract - GameObject - Toggle``` -> OnInteract-GameObject-Toggle.asset\
```OnEnable   - GameObject - On    ``` -> OnEnable-GameObject-On.asset

| Prefix |  |  |  |
| :--- | :--- |  :--- | :--- |
|```On...``` | Non-synced Triggers | Found in "Regular Udon-Graph-Triggers" | Set Synchronization to 'None'|
|```Sync_On...``` | Synced Triggers | Found in "Synced Udon-Graph-Triggers"| Set Synchronization to 'Manual'|

| Event |  |
| :--- | :--- |
|On Enable | As soon as the Object is enabled, often used to activate on World being loaded.|
|On Enter Station | When entering a Seat|
|On Exit Station | When leaving a Seat|
|On Interact | When interacting with a Button or similar|
|On Object PickUp | When an Object is picked up|
|On Object Drop | When a held Object is dropped|
|On Object Enter Trigger | When Objects enter a trigger area that they share a Layer with |
|On Object Exit Trigger | When Objects exit a trigger area that they share a Layer with|
|On Player Enter Trigger | When entering a trigger area|
|On Player Exit Trigger | When exiting a trigger area|
|On Player joined | When any Player joins |

| Affecting |  |
| :--- | :--- |
|GameObject | "targets" can be multiple ones. A number of targets above 1 needs to be input to use more than 1.|
|AnimatorBool | target here is the GameObject that has the Animator component.|
|Collider | target here is the GameObject, it will select the Collider automatically.|
|Collider IsTrigger | target here is the GameObject, it will select the Collider automatically and adjust its "IsTrigger" state.|

| State |  |
| :--- | :--- |
|On||
|Off||
|Toggle||
|On then Off| Sets the state to On and then to Off, with a field to set a delay inbetween.|
|Off then On| Sets the state to Off and then to On, with a field to set a delay inbetween.|

| Misc |  |
| :--- | :--- |
|LocalPlayer | Only triggers on your own Player, not when other Players interact|
|RandomChance | These triggers only fire at random.| A chance between 0.0 (never) to 1.0 (always) can be set|
|Delayed | These triggers have a field to set a delay for the action.|

Requirements:
Only the VRChat SDK

Nodes are set at the same position on the graph across all behaviours found here. This means Events, SetActive and other nodes that occur multiple times across multiple scripts are always found at the same spot.
These behaviours run entirely on vanilla Udon Graph and require no UdonSharp and no other dependencies to work. They exist to remove dependency of 3. parties to continue maintaining their projects.
Simple triggers should only need simple requirements.

I developed these as part of my efforts to make maintaining my VRChat Worlds as easy as possible. Having to rely on anything other than the VRChat SDK and potentially replacing tools can be a time drain in the future that is easily avoidable.

~Maebbie

*[initital release 2024-08-01](https://github.com/Maebbie/Udon-Graph-Triggers/activity?sort=ASC)*
