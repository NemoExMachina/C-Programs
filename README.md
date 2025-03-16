<html>
    <head>
        <title>String and Array</title>
        <style>
            body {
                font-family: Arial, sans-serif;
                background-color: #f3f3f3;
                color: #333;
                margin: 0;
                padding: 0;
                line-height: 1.6;
            }
            .code-container {
                background-color: #282c34;
                color: #61dafb;
                padding: 16px;
                border-radius: 8px;
                font-family: Consolas, "Courier New", monospace;
            }
            .code-container span.keyword {
                color: #d19a66;
                font-weight: bold;
            }
        </style>
    </head>
    <body>
        <div class="code-container">
            <h2>Program to check whether entered number is even or odd.</h2>
            <pre>
    #include<<span class="keyword">stdio</span>.h&gt;
    <span class="keyword">int</span><span class="function"> main</span>() {
    <span class="keyword">int</span> a;
    printf(<span class="string">"Enter any no. ?"</span>);
    scanf(<span class="string">"%d"</span>, &a);
    <span class="keyword">if</span>(a%2==0) {
        printf(<span class="string">"\nEven no."</span>);
    }
    <span class="keyword">else</span> {
         printf(<span class="string">"\nOdd no."</span>);
    }
    <span class="keyword">return</span> 0;}
    }
    <br>
    <img src="C:\Users\Admin\Documents\Binay's Assignments\024NEB840__assignment1\HTML\Programs\Odd.png" alt="Output" width="350" height="80">
    <img src="C:\Users\Admin\Documents\Binay's Assignments\024NEB840__assignment1\HTML\Programs\Even.png" alt="Output" width="350" height="80">
        <div class="code-container">
            <h2>String Handling Functions</h2>
            <pre>
    <h3>1. strlen() - Length of string</h3>
    #include<<span class="keyword">stdio</span>.h&gt;
    #include<<span class="keyword">string</span>.h&gt;
    <span class="keyword">int</span><span class="function"> main</span>() {
    <span class="keyword">char</span> a[100], b[100], result[200];
    printf(<span class="string">"Enter the first string ?"</span>);
    scanf(<span class="string">"%s"</span>, a);
    printf(<span class="string">"Enter the second string ?"</span>);
    scanf(<span class="string">"%s"</span>, b);
    <span class="keyword">int</span> c, d;
    c = strlen(a);
    d = strlen(b);
    printf(<span class="string">"\nLength of string 1: %d\n"</span>, c);
    printf(<span class="string">"Length of string 2: %d\n"</span>, d);
    <span class="keyword">if</span>(c > d) {
        printf(<span class="string">"\nString 1 is longer."</span>);
    }<span class="keyword">else</span> <span class="keyword">if</span>(c < d) {
        printf(<span class="string">"\nString 2 is longer."</span>);
    }<span class="keyword">else</span> {
    printf(<span class="string">"\nBoth strings are of equal length."</span>);
    }
    <h3>2. strlwr() - Convert to lowercase</h3>
    <span class="keyword">char</span> temp1[100], temp2[100];
    printf(<span class="string">"\nString 1 in lowercase: %s\n"</span>, strlwr(a));
    printf(<span class="string">"String 2 in lowercase: %s\n"</span>, strlwr(b));   
    <h3>3. strupr() - Convert to uppercase</h3>
    printf(<span class="string">"\nString 1 in uppercase: %s\n"</span>, strupr(a));
    printf(<span class="string">"String 2 in uppercase: %s\n"</span>, strupr(b));   
    <h3>4. strcpy() - Copy strings</h3>
    strcpy(temp1, a);
    printf(<span class="string">"\nCopied string 1 to temp1: %s\n"</span>, temp1); 
    <h3>5. strcmp() - Compare strings</h3>
    <span class="keyword">int</span> R = strcmp(a, b);
    <span class="keyword">if</span> (R == 0) {
        printf(<span class="string">"\nStrings are equal.\n"</span>);
    } 
    <span class="keyword">else</span> {
        printf(<span class="string">"\nString 1 is not equal to String 2.\n"</span>);
    }    
    <h3>6. strcat() - Concatenate strings</h3>
    strcpy(result, a); // Copy a to result
    strcat(result, b); // Append b to result
    printf(<span class="string">"\nConcatenated string: %s\n"</span>, result);  
    <h3>7. strrev() - Reverse string</h3>
    printf(<span class="string">"\nReversed String 1: %s\n"</span>, strrev(a));
    printf(<span class="string">"Reversed String 2: %s\n"</span>, strrev(b));
    <span class="keyword">return</span> 0;
    </pre>
    </div>
    <img src="C:\Users\Admin\Documents\Binay's Assignments\024NEB840__assignment1\HTML\Programs\String.png" alt="Output" width="400" height="400">
    <div class="code-container"></div>
        <h1>1D Number Array and 1D Character Array</h1>
        <pre>
    #include<<span class="keyword">stdio</span>.h&gt;
    <span class="keyword">int</span><span class="function"> main</span>() {
        <span class="keyword">int</span> numbers[5] = {1, 2, 3, 4, 5};
        <span class="keyword">char</span> characters[6] = "hello";
        printf(<span class="string">"Number Array: "</span>);
        <span class="keyword">for</span>(<span class="keyword">int</span> i = 0; i < 5; i++) {
            printf(<span class="string">"%d "</span>, numbers[i]);
        }
        printf(<span class="string">"\nCharacter Array: %s\n"</span>, characters);
        <span class="keyword">return</span> 0;
    }
        </pre>
        <img src="C:\Users\Admin\Documents\Binay's Assignments\024NEB840__assignment1\HTML\Programs\1D-Array.png" alt="Output" width="390" height="200">
    <div class="code-container"></div>
        <h1>2D Number Array and 2D Character Array</h1>
        <pre>
    #include<<span class="keyword">stdio</span>.h&gt;
    <span class="keyword">int</span><span class="function"> main</span>() {
        <span class="keyword">int</span> numbers[2][3] = {
            {1, 2, 3},
            {4, 5, 6}
        };
        <span class="keyword">char</span> characters[2][10] = {
            "hello",
            "world"
        };
        printf(<span class="string">"2D Number Array:\n"</span>);
        <span class="keyword">for</span>(<span class="keyword">int</span> i = 0; i < 2; i++) {
            <span class="keyword">for</span>(<span class="keyword">int</span> j = 0; j < 3; j++) {
                printf(<span class="string">"%d "</span>, numbers[i][j]);
            }
            printf(<span class="string">"\n"</span>);
        }
        printf(<span class="string">"\n2D Character Array:\n"</span>);
        <span class="keyword">for</span>(<span class="keyword">int</span> i = 0; i < 2; i++) {
            printf(<span class="string">"%s\n"</span>, characters[i]);
        }
        <span class="keyword">return</span> 0;
    }
        </pre>
        <img src="C:\Users\Admin\Documents\Binay's Assignments\024NEB840__assignment1\HTML\Programs\2D-Array.png" alt="Output" width="390" height="250">
    </div>
    </body>
</html>
![1D-Array](https://github.com/user-attachments/assets/33cbb19a-daa0-4e0e-afc8-2f85e67fad9a)
![2D-Array](https://github.com/user-attachments/assets/06aef6a4-c2bb-418c-8e28-d96709825958)
