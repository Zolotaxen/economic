# economic
def calculate_growth_rate(initial_gdp, final_gdp, num_years):
    growth_rate = ((final_gdp / initial_gdp) ** (1 / num_years)) - 1
    return growth_rate

def main():
    initial_gdp = float(input("Enter the initial GDP: "))
    final_gdp = float(input("Enter the final GDP: "))
    num_years = int(input("Enter the number of years: "))

    growth_rate = calculate_growth_rate(initial_gdp, final_gdp, num_years)
    print("The GDP growth rate is:", "{:.2%}".format(growth_rate))

if __name__ == "__main__":
    main()
