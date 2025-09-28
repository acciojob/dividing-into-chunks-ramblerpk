<!DOCTYPE html>
<html>
<head>
    <title>Array Chunking by Maximum Sum</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            max-width: 800px;
            margin: 0 auto;
            padding: 20px;
            background-color: #f5f5f5;
        }
        .container {
            background-color: white;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }
        h1 {
            color: #333;
            text-align: center;
            margin-bottom: 30px;
        }
        .input-section {
            margin-bottom: 30px;
            padding: 20px;
            background-color: #f8f9fa;
            border-radius: 8px;
        }
        .input-group {
            margin-bottom: 15px;
        }
        label {
            display: block;
            margin-bottom: 5px;
            font-weight: bold;
            color: #555;
        }
        input {
            width: 100%;
            padding: 10px;
            border: 2px solid #ddd;
            border-radius: 5px;
            font-size: 16px;
        }
        input:focus {
            border-color: #007bff;
            outline: none;
        }
        button {
            background-color: #007bff;
            color: white;
            padding: 12px 24px;
            border: none;
            border-radius: 5px;
            font-size: 16px;
            cursor: pointer;
            transition: background-color 0.3s;
        }
        button:hover {
            background-color: #0056b3;
        }
        .result-section {
            margin-top: 30px;
            padding: 20px;
            background-color: #e8f5e8;
            border-radius: 8px;
            border-left: 4px solid #28a745;
        }
        .result-section h3 {
            color: #155724;
            margin-top: 0;
        }
        .chunk {
            background-color: #fff;
            border: 1px solid #28a745;
            border-radius: 5px;
            padding: 10px;
            margin: 5px 0;
            font-family: monospace;
        }
        .example-section {
            margin-top: 30px;
            padding: 20px;
            background-color: #fff3cd;
            border-radius: 8px;
            border-left: 4px solid #ffc107;
        }
        .example-section h3 {
            color: #856404;
            margin-top: 0;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Array Chunking by Maximum Sum</h1>
        
        <div class="input-section">
            <div class="input-group">
                <label for="arrayInput">Enter array (comma-separated numbers):</label>
                <input type="text" id="arrayInput" value="1, 2, 3, 4, 1, 0, 2, 2" placeholder="e.g., 1, 2, 3, 4, 1, 0, 2, 2">
            </div>
            <div class="input-group">
                <label for="maxSum">Enter maximum sum (n):</label>
                <input type="number" id="maxSum" value="5" placeholder="e.g., 5">
            </div>
            <button onclick="runDivide()">Divide Array</button>
        </div>
        
        <div id="results" style="display: none;" class="result-section">
            <h3>Result:</h3>
            <div id="resultContent"></div>
        </div>
        
        <div class="example-section">
            <h3>Examples:</h3>
            <p><strong>Input:</strong> [1, 2, 3, 4, 1, 0, 2, 2], n = 5</p>
            <p><strong>Output:</strong> [[1, 2], [3], [4, 1, 0], [2, 2]]</p>
            <p><strong>Input:</strong> [4, 3, 2, 1], n = 4</p>
            <p><strong>Output:</strong> [[4], [3], [2, 1]]</p>
        </div>
    </div>

    <script>
        const divide = (arr, n) => {
            const result = [];
            let currentChunk = [];
            let currentSum = 0;
            
            for (let i = 0; i < arr.length; i++) {
                const element = arr[i];
                
                // If adding this element would exceed the maximum sum
                if (currentSum + element > n) {
                    // If we have elements in current chunk, push it to result
                    if (currentChunk.length > 0) {
                        result.push([...currentChunk]);
                    }
                    // Start a new chunk with current element
                    currentChunk = [element];
                    currentSum = element;
                } else {
                    // Add element to current chunk
                    currentChunk.push(element);
                    currentSum += element;
                }
            }
            
            // Don't forget to add the last chunk if it's not empty
            if (currentChunk.length > 0) {
                result.push(currentChunk);
            }
            
            return result;
        };

        function runDivide() {
            const arrayInput = document.getElementById('arrayInput').value;
            const maxSumInput = document.getElementById('maxSum').value;
            
            try {
                // Parse the array input
                const arr = arrayInput.split(',').map(x => parseInt(x.trim()));
                const n = parseInt(maxSumInput);
                
                // Validate inputs
                if (arr.some(isNaN) || isNaN(n)) {
                    throw new Error('Please enter valid numbers');
                }
                
                if (n <= 0) {
                    throw new Error('Maximum sum must be positive');
                }
                
                // Check constraint: max value in array should be <= n
                const maxValue = Math.max(...arr);
                if (maxValue > n) {
                    throw new Error(`Maximum value in array (${maxValue}) exceeds the maximum sum limit (${n})`);
                }
                
                // Run the divide function
                const result = divide(arr, n);
                
                // Display results
                displayResults(arr, n, result);
                
            } catch (error) {
                alert('Error: ' + error.message);
            }
        }

        function displayResults(arr, n, result) {
            const resultsDiv = document.getElementById('results');
            const resultContent = document.getElementById('resultContent');
            
            let html = `
                <p><strong>Input Array:</strong> [${arr.join(', ')}]</p>
                <p><strong>Maximum Sum:</strong> ${n}</p>
                <p><strong>Number of Chunks:</strong> ${result.length}</p>
                <h4>Chunks:</h4>
            `;
            
            result.forEach((chunk, index) => {
                const sum = chunk.reduce((a, b) => a + b, 0);
                html += `<div class="chunk">Chunk ${index + 1}: [${chunk.join(', ')}] (sum: ${sum})</div>`;
            });
            
            html += `<p><strong>JSON Output:</strong> ${JSON.stringify(result)}</p>`;
            
            resultContent.innerHTML = html;
            resultsDiv.style.display = 'block';
        }

        // Test with the provided examples on page load
        window.onload = function() {
            // Test case 1
            console.log('Test 1:', divide([1, 2, 3, 4, 1, 0, 2, 2], 5));
            // Expected: [[1, 2], [3], [4, 1, 0], [2, 2]]
            
            // Test case 2
            console.log('Test 2:', divide([4, 3, 2, 1], 4));
            // Expected: [[4], [3], [2, 1]]
        };
    </script>
</body>
</html>