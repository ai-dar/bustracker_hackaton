# Bus Stop Forecasting and Visualization

This project is a simulation and visualization of bus stop arrival forecasting using Python, with a GUI implemented in both Tkinter and Pygame. It generates a forecast based on random travel times between stops, displays this information in a Tkinter window, and visualizes the bus route in Pygame.

## Features

- **Tkinter Forecast Display**: Shows estimated arrival times for each bus stop in a scrollable window.
- **Pygame Visualization**: Visualizes the bus moving along a route, with interactive bus stops.
- **Dynamic Route Generation**: Randomly generates a bus route with 3 to 8 stops and calculates cumulative travel times for each segment.
- **Interactive Bus Stops**: Clicking on a stop in the Pygame window displays remaining time to arrival at that stop.

## Installation

### Prerequisites

- **Python 3.6+**
- **Pygame**: `pip install pygame`
- **Pandas**: `pip install pandas`
- **Tkinter**: Typically included with Python, but you may need to install it separately based on your OS.
- **Dotenv**: `pip install python-dotenv` (for loading API keys)

### Setup

1. **Clone this repository**:
    ```bash
    git clone <repository-url>
    cd <repository-name>
    ```

2. **Install the required packages**:
    ```bash
    pip install -r requirements.txt
    ```

3. **Configure API keys**:
    - Create a `.env` file in the project root.
    - Add your API keys in this format:
      ```plaintext
      GEMINI_API_KEY=your_gemini_api_key
      GOOGLE_API_KEY=your_google_api_key
      ```

4. **Place images**:
   - Add `bus.png` and `bus_stop.png` images to the project root or specify the correct paths if they are stored elsewhere.

## Usage

1. **Run the script**:
    ```bash
    python <script-name>.py
    ```

2. **Tkinter Window**:
   - Displays the forecasted arrival times for each bus stop in a scrollable window.

3. **Pygame Window**:
   - Shows a map with bus stops and routes.
   - Click on a stop to see the remaining time until arrival.

## Code Structure

- **Forecast Calculation**: Generates random travel times between stops and forecasts arrival times.
- **Tkinter GUI**: A scrolled text area to display arrival forecasts.
- **Pygame GUI**: Visualizes the bus route and shows interactive stops.
  
## Customization

- **Change the number of stops**: Adjust the `num_stops` variable to control the range of stops generated.
- **Modify bus and stop sizes**: Change dimensions in `pygame.transform.scale` for `bus_image` and `stop_image` to resize the images.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

