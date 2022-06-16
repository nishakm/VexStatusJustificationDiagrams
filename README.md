This repo is to update the diagrams being used in the VEX document.

The diagrams are made with draw.io.
They are png's with the draw.io source included,
so they can be edited directly with draw.io.

Release v0.1.0 are the files as reviewed at the 2022-06-13 VEX Meeting.

The files were renamed to the sections of the document in which they appear.

The "a" version is the original as reviewed.

The "b" version is the changes requested at the meeting.

If a "c" version exists, it is to show an alernative way (eg I wasn't sure which was decided at meeting so I did both).

3.2-Legend.b.drawio.png has the following changes:
- it is no longer 'empty', it is the 'code is vulnerable' case
- per Charlie's suggestion, just the software is colored not the component. This is obviously the oversimplified example of:
   + one product
   + with 3 components,
   + each component has only one software module/library (note there will be one exception to this later that will have two modules)
   + two components are vuln-free and one component has a vulnerability that is exploitable.
- the vulnerability is shown as a red X (so it's a vulnerability in a module in a software product)

3.3-component_not_present.b has changes similar to 3.2. Note no orange modules, no red X's.

3.4-vulnerable_code_not_present.b has changes similar to 3.2. Note component does NOT have red X but is "in" the orange. Ie the CVE called out that component but in this case the vulnerable code was compiled out

3.5-vulnerable_code_not_in_execute_path.b has changes similar to 3.2. The red X makes it more obvious the bad code is there, just not executed.

3.6-vulnerable_code_cannot_be_controlled_by_adversary.b has changes similar to 3.2. It also has Eliot's proposed change to move adversary to the top

3.7-inline_mitigations_exist.b has changes similar to 3.2. It also has
Duncan's proposed change to 'enclose' with mitigations. 3.7-inline_mitigations_exist.c is a different version (just the component) in case people like that better.
