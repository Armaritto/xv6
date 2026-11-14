# xv6

This repository contains starter code and instructions for xv6 labs.

## Repository branches

| Branch | Contents |
|--------|----------|
| main | General instructions |
| fs | Large-file lab |
| pgtbl | Page-table lab |

## Lab goals

### Page tables — branch `pgtbl` 

- Inspect a process's page-table mappings and explain their permissions.
- Provide a read-only shared page containing the process ID.
- Implement vmprint() to display the page-table tree.

### File system — branch `fs`

- Extend xv6 to support larger files using doubly-indirect blocks.
- Your implementation must support writing and reading 65,803 data blocks
and correctly free allocated blocks when files are deleted or truncated.


## Workflow

1. Select **Use this template → Create a new repository**.
2. Choose **Private** and enable **Include all branches**.
3. Clone that private repo
4. Switch to the assigned lab branch
5. Implement and test one change at a time
6. Commit your work regularly
7. Run the relevant tests to check your work
8. Run `usertests -q` before submission to check that existing OS behavior still works.
9. Run the grader to check your score before submission


## Build and run

From the assigned lab branch, run these commands in your Linux terminal:

```bash
make clean
make qemu
```

Inside xv6, run the test for your assigned lab:

- `pgtbl` branch: `pgtbltest`
- `fs` branch: `bigfile`


Run the regression tests inside xv6:

```text
usertests -q
```

To exit QEMU, press Ctrl+A, release, then press X.

To run the lab grader, exit QEMU and run this in your Linux terminal:

```bash
make grade
```

Some tests intentionally fail on the starter because the required
features have not been implemented yet.

## Policy

- Complete these labs independently
- Do not use AI tools to generate solution code
- Do not copy solution code from online resources or other students
- Keep your solution repository private to prevent others from accessing or copying your work
