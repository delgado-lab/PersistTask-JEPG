**Description of Task Files for "PersTaskfmri"**

**Used in publications**:

> Bhanji, Kim, & Delgado (2016 - pdf of manuscript and supplement are included in this repository as "BhanjiKimDelgado2016.pdf" and "BhanjiKimDelgado2016JEPG_Supplement.pdf"), also see Bhanji & Delgado (2014)

**Important Filenames (in the TaskFiles folder):**

> *PersTask_Instruct_UncCon.es2, PersTask_Instruct_UncCon_reversed.es2*
> -- e-prime files for instructions and practice rounds -- \*\_reversed
> is the same, but with colors of stimuli switched.
>
> *PersTask_UncCon_selfpaced.es2,
> PersTask_UncCon_reversed_selfpaced.es2--* e-prime main task file --
> \*\_reversed is the same, but with colors of stimuli switched
>
> *images* - folder of images needed for the e-prime presentation

**File Descriptions**

***PersTask_Instruct_UncCon.es2:*** Eprime 2.0 file -- Instructions &
practice to go with *PersTask_UncCon_selfpaced.es2 main experiment
file*.

***PersTask_Instruct_UncCon_reversed.es2:*** Eprime 2.0 file --
Instructions & practice to go with
*PersTask_UncCon_reversed_selfpaced.es2 main experiment file*.

***PersTask_UncCon_selfpaced.es2 &
PersTask_UncCon_reversed_selfpaced.es2:***

*Experimental Design:* 2 conditions within subjects (Condition changes
from round to round, but not within)

> Conditions: Uncontrollable Obstacles, Controllable Obstacles, Progress
> Events - participant receives same pattern of obstacle setbacks in
> both conditions.

-   Uncontrollable Obstacles (purple triangle (orange in reversed
    version) - setbacks framed as random)

-   Controllable Obstacles (orange triangle (purple in reversed
    version) - setbacks due to "incorrect" response)

-   Progress Cues (green triangle)

*Timing Information:*

> Event Timing - Path Choice (terminates with response), self-paced
> Obstacle Cue (terminates with response), 4s Fixation, 2s Obstacle
> Outcome (Setback received/avoided), 4/6s (50/50%) Fixation (\*no
> fixation between cue and outcome for Progress Cues)

*Trial Counts and other details:*

> 12 rounds, 40 obstacle cues, 24 setbacks and 16 avoided setbacks (60%
> of obstacles result in setback), 24 persistence choices (after each
> setback), 16 progress cues-- divided equally across the 2 conditions

*How to interpret output files:*

> EventType: 1=uncontrollable obstacle, 2=controllable obstacle,
> 3=progress cue, 4=path choice, 6=goal feedback
>
> Lose: 1=setback received, 0=setback avoided, -1=event was path choice
> or goal feedback
>
> Persist: 1 = choice to try again on the same path where a setback was
> just experienced, 0 = choice to switch to a different path than the
> one where the setback was experienced, -2=first path choice of the
> round, not included in persistence calculation, -1 = no response given
> for path choice

**Other notes (e.g., how to calculate behavioral measures, other
versions of the task that might be helpful)**

> To calculate Behavioral Persistence for each participant, you take the
> number of Persist choices (coded as "1" in the "Persist" column of
> output for each condition, and divide by the total number of
> post-setback choices (choices with a "1" or "0" in the Persist column.
> Missed choices have a "-2" in the "Persist" column).
>
> The "Switch" column in the output has value "1" when the participant
> chooses a path that is lower in value than the current path, "0" if
> they choose the same path or a higher value path.
>
> The files named "PathTask" in the SmokPersist and Opiod study folders
> are designed to be easier to share (and are shorter versions of the
> task, without Academic framing).
>
> If a participant does not change their response after a controllable
> setback (i.e., fails to learn from a mistake), then a setback is
> received and the study continues on.
