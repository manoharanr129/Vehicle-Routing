# Vehicle Routing Problem (VRP) Optimization using Genetic Algorithm

## Overview
This project implements a **Genetic Algorithm (GA)** to solve the **Vehicle Routing Problem (VRP)** with multiple vehicles. The goal is to minimize the total distance traveled while balancing the workload among vehicles.

## Features
- Uses **Genetic Algorithm (GA)** for optimization.
- Supports multiple vehicles.
- Visualizes optimal routes using **Matplotlib**.
- Evaluates fitness based on total distance and balance penalty.
- Implements **crossover, mutation, and selection** operators.

## Requirements
To run this project, install the necessary dependencies:
```sh
pip install matplotlib==3.7.2 deap==1.3.3
```

## How It Works
1. **Randomly generate locations** (excluding the depot) for vehicles to visit.
2. **Define a genetic algorithm** with:
   - **Permutation-based representation** (shuffled indices of locations)
   - **Crossover (PMX), mutation (shuffle), and tournament selection**
3. **Evaluate fitness** based on:
   - **Total distance** traveled by all vehicles.
   - **Balance penalty**, using standard deviation of distances per vehicle.
4. **Evolve the population** over generations to find the best routes.
5. **Visualize the optimized routes**.

## Code Structure
- **Define problem parameters**: Number of vehicles, depot location, and random locations.
- **Genetic Algorithm setup**: Chromosome representation, fitness function, genetic operators.
- **Visualization function**: Plots optimized vehicle routes.
- **Main function**: Runs the GA and prints the best solution.

## Running the Program
To execute the program, follow these steps:
1. Clone the repository:
   ```sh
   git clone https://github.com/your-repo/vrp-ga.git
   cd vrp-ga
   ```
2. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```
3. Run the script:
   ```sh
   python vrp_ga.py
   ```

## Example Output
```
Best individual: [3, 7, 1, 5, 8, 2, 6, 0, 4, 9]
Best fitness: (245.67, 12.45)
```
A visualization of the best route is displayed.

## Visualization
The final output includes a plot showing:
- **Depot location (black square)**
- **Customer locations (circles)**
- **Optimized routes for each vehicle (colored lines)**

### Example Output Image
![Optimized VRP Route](images/VRP.png)

> **Note:** Ensure the output image is saved in the `images` folder inside your repository.

## Future Enhancements
- Implement **real-world constraints** (vehicle capacity, time windows).
- Use **advanced crossover/mutation** strategies.
- Experiment with **hybrid optimization techniques**.
- Optimize **runtime efficiency** by parallelizing computations.
- Implement **dynamic route adjustments** based on real-time changes.

## License
This project is open-source under the **MIT License**.

## Contributions
Contributions are welcome! Feel free to submit issues or pull requests to improve the algorithm or add new features.

## Contact
For any questions or collaborations, reach out via [GitHub Issues](https://github.com/your-repo/issues) or email at example@example.com.
