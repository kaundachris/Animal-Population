class AnimalPopulation:
    def __init__(self, max_population: int, present_population: int, birth_rate: float):
        self.present_population = present_population
        self.max_population = max_population
        self.generations = 1000
        self.birth_rate = birth_rate

    def population_change(self):
        x = self.present_population/self.max_population
        i = 0
        list_populations = []
        while i < self.generations:
            new_population = (self.birth_rate * x) * (1 - x)
            x = new_population
            if self.generations - 20 < i < self.generations:
                list_populations.append(round(x, 3))
            i += 1
        return list_populations
