# AI Project: Timetable Scheduling

## Overview

This project is part of the Artificial Intelligence course, focused on solving the timetable scheduling problem in a university environment. The goal is to create a timetable for each semester that minimizes clashes between sections, professors, and rooms.

## Project Description

The timetable scheduling problem involves assigning time slots to each section in a particular room to be taught by a specific professor. The solution must satisfy a set of hard constraints and optimally address soft constraints.

### Hard Constraints

1. Classes can only be scheduled in free classrooms.
2. Classrooms must be large enough to accommodate the section.
3. A professor cannot be assigned to two different lectures at the same time.
4. The same section cannot be assigned to two different rooms at the same time.
5. A room cannot be assigned to two different sections at the same time.
6. No professor can teach more than three courses.
7. No section can have more than five courses in a semester.
8. Each course must have two lectures per week, not on the same or adjacent days.
9. Lab sessions should be conducted in two consecutive slots.
10. There should be 15-minute breaks between consecutive classes.

### Soft Constraints

1. Theory classes should be taught in the morning, and lab sessions should be in the afternoon.

## Timetable Details

- The timetable covers five days of the week.
- Morning session: 8:30 AM – 2:30 PM
- Afternoon session: 2:30 PM – 5:30 PM

## Genetic Algorithm Implementation

The solution uses a genetic algorithm with the following steps:

1. **Initial Population**: Random bitstrings representing the timetable.
2. **Evaluation**: Fitness function to minimize clashes.
3. **Selection**: Roulette Wheel selection to choose parents.
4. **Crossover**: Recombination of parents to create children.
5. **Mutation**: Randomly flipping bits in the bitstring.
6. **Iteration**: Repeating the process for a set number of generations.

### Key Functions

- **Selection**: Selects the best candidates for reproduction.
- **Crossover**: Combines parents to create offspring.
- **Mutation**: Introduces variability by flipping bits.

## Requirements

- Python programming language
