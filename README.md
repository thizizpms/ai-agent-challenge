# AI Agent for Bank Statement PDF Parsing - Karbon Challenge

## 5-Step Run Instructions

1. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

2. **Set up API key:**
   ```bash
   export GEMINI_API_KEY="your_api_key_here"
   ```

3. **Prepare sample data:**
   - Place PDF at `data/{bank_name}/{bank_name}_sample.pdf`
   - Place CSV at `data/{bank_name}/{bank_name}_sample.csv`

4. **Run the agent:**
   ```bash
   python agent.py --target {bank_name}
   ```

5. **Use generated parser:**
   - Find parser at `custom_parsers/{bank_name}_parser.py`

## Agent Architecture

The agent follows a plan → analyze → generate → test loop that adapts to different bank formats.
