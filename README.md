# flask-shopify-app

To run the application:

### 1. Clone the Repository

Clone the repository to your local machine:

```bash
git clone https://github.com/universalbrother/flask-shopify-app.git
cd flask-shopify-app

### 2. Create a Virtual Environment

Create and activate a virtual environment:

#### On Windows:

```bash
python -m venv venv
venv\Scripts\activate

#### On mac and linux:

python3 -m venv venv
source venv/bin/activate

### 3. Install Required Packages

Install the required packages using `pip`:

```bash
pip install Flask requests notebook

### 4. Open the Jupyter Notebook

Open the Jupyter Notebook to run the Flask application:

```bash
jupyter notebook flask_shopify_clean.ipynb

### 5. Run All Cells

Run all cells in the notebook to start the Flask application. The application will be served at `http://127.0.0.1:5000`.

## Endpoints

The following endpoints are available in the application:

- `/` - Home route with a welcome message.
- `/orders` - Fetch the number of orders.
- `/order/<order_id>` - Fetch product names and inventory status for a specific order ID.
- `/mock_shipbob_order` - Print a mocked Shipbob API request to the console.
- `/list_orders` - List all order IDs.

### Example Usage

1. **Fetch Number of Orders**

   Navigate to `http://127.0.0.1:5000/orders` to get the number of orders in the Shopify store.

2. **Fetch Order Details**

   Navigate to `http://127.0.0.1:5000/order/<order_id>` (replace `<order_id>` with a valid order ID) to fetch the product names and inventory status for that order.

3. **Mock Shipbob API Request**

   Navigate to `http://127.0.0.1:5000/mock_shipbob_order` to print a mocked Shipbob API request to the console.

4. **List Orders**

   Navigate to `http://127.0.0.1:5000/list_orders` to list all order IDs.

## Notes

- If at any point it throws an error please restart the kernel and run the cells sequentialy again.
- **Order #1028 is not a real order** :))

## Project Structure

- `flask_shopify_clean.ipynb`: Jupyter Notebook containing the Flask application code.
- `README.md`: This file.
- `.gitignore`: Git ignore file to exclude unnecessary files from the repository.

## Author
Daniel Iahr