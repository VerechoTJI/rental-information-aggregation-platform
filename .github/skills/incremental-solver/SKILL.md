---
name: incremental-solver
description: Solve RIAP work using an incremental four-stage model. Use when you want to work one PBI at a time, move it to active, understand it together, plan small tasks, and commit after each completed task.
---

# Incremental Solver Skill

Use this skill when a task should be solved one PBI at a time in small, safe increments.

## When To Use

- When the work is multi-step or ambiguous.
- When the user wants a process model for solving PBIs.
- When you need a repeatable way to move from PBI intake to completion.

## Step-by-Step Guide

1. **Select one PBI**
   - Work on only one PBI at a time.
   - If the PBI is pending, move it to `pbi/active/` before doing any implementation.

2. **Review it together**
   - Read the PBI and the relevant requirements.
   - Update the PBI with any new knowledge, clarification, or scope change.

3. **Break it into tasks**
   - Split the feature into the smallest useful steps.
   - Write the steps in the PBI as a checklist.

4. **Create a planning commit**
   - Make a commit after the PBI is understood and the task list is ready.
   - Keep this commit focused on setup and planning, not feature completion.

5. **Do one task at a time**
   - Complete the first task only.
   - Keep the change small and focused.

6. **Commit the completed task**
   - Make a commit after each completed task.
   - Keep each commit tied to one task or one small coherent increment.

7. **Verify and continue**
   - Run tests or other checks after the task is done.
   - If more tasks remain, repeat steps 5–7 until the PBI is finished.

8. **Run TDD and update related files**
   - Run the test-first cycle for the completed work or the next failing behavior.
   - Update the related files based on the test results and any new knowledge.
   - Keep the PBI checklist, notes, and traceability entries in sync with the code changes.

9. **Final review and close out**
   - Review the completed PBI together one last time.
   - Move the PBI file to `pbi/done/` when all tasks are finished and accepted.
   - Make a closing commit that captures the completed PBI and any final adjustments.

## PBI Flow

1. **Pick One PBI**
   - Work on a single PBI only.
   - If the PBI is pending, move it to `pbi/active/` before implementation starts.

2. **Understand Together**
   - Review the PBI with the user or the available requirements.
   - Update the PBI file with new knowledge, clarifications, or traceability notes.

3. **Plan the Task List**
   - Break the PBI into small tasks.
   - Turn features into the smallest useful actionable steps.
   - Create a checkpoint commit after the plan is set up, before carrying out the work.

4. **Execute One Task at a Time**
   - Complete tasks sequentially.
   - Commit after each completed task.
   - Keep each commit focused on one task or one small coherent increment.

## Four Stages

1. **Understand**
   - Restate the problem and identify the desired outcome.
   - Note constraints, inputs, outputs, and anything that is missing.

2. **Plan**
   - Break the work into the smallest useful increments.
   - Decide the order of implementation and what success looks like for each increment.

3. **Implement**
   - Complete one increment at a time.
   - Keep each change focused and avoid mixing unrelated work.

4. **Verify**
   - Check the result against the original goal.
   - Run tests or other validation steps when available.

## Incremental Rules

- Never work on more than one PBI at the same time.
- Move a PBI to `active` as soon as implementation begins.
- Update the PBI file as new knowledge is discovered.
- Commit once after planning is ready, then commit after each completed task.
- After the last task, do a final review together, move the PBI to `done`, and make a closing commit.
- Run TDD at the end of the task flow and update related files before the final review.
- Prefer the smallest useful change that moves the work forward.
- Keep each increment independently understandable.
- Do not skip verification between major steps.
- If a step fails, adjust only the current increment before moving on.

## Response Pattern

- Start by identifying the current PBI.
- Summarize what is understood and what needs clarification.
- Update the PBI file with any new knowledge.
- Present the next small task.
- Make the change, commit it, and verify it before continuing.
- When the PBI is complete, perform a final review, move it to `done`, and make the closing commit.
- After the final task, run TDD, update related files, then do the final review and closeout.

## Example Usage

- Use this skill to solve a feature request by selecting one PBI, moving it to active, understanding it together, planning the smallest next tasks, creating a planning commit, executing and committing each task one by one, running TDD and updating related files at the end, and then doing a final review before moving the PBI to done and making the closing commit.
