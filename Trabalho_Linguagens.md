## Trabalho de Linguagens de Programação Comparadas

### Roteiro de apresentação

#### Responder às seguintes perguntas:

+ Qual o [paradigma](https://en.wikipedia.org/wiki/Programming_paradigm) da linguagem escolhida?
    
    Paradigma de programação: É a forma como uma linguagem de programação é criada. Como a mesma solução pode ser pensado de uma forma  diferente... A princípio a linguagem era binária, não precisava ser traduzida mas não era prática... Daí surgiu o assembly e as pessoas começaram a gostar da brincadeira...
    No caso do JAVA o paradigma é a "orientação à objeto"

+ Seu código é [interpretado](https://en.wikipedia.org/wiki/Interpreted_language) ou [compilado](https://en.wikipedia.org/wiki/Compiled_language)?

    
+ Qual a ["tipagem"](https://en.wikipedia.org/wiki/Strong_and_weak_typing) da linguagem?

    
+ Quais são suas principais vantagens e desvantagens. Mostre também os [domínios principais de aplicação](https://tomassetti.me/best-programming-languages/)?
    
        Vantagens:
            - Frameworks
            - Multiplataforma (Máquina Virtual)
            - Linguagem mais usada no planeta
        Desvantagens:
            - Lenta
            - Garbage collector error

    
+ Cite os [tipos primitivos de dados](https://en.wikipedia.org/wiki/Primitive_data_type) da linguagem escolhida.

    
+ Mostre como são as estruturas de [controle de fluxo](https://en.wikipedia.org/wiki/Control_flow).  

    
+ Mostre, na linguagem escolhida, o código necessário para as seguintes tarefas:  
  + Olá mundo: O objetivo desse problema é que, ao ser executado, ele nos retorne na tela a frase “Olá
Mundo”, e seja finalizado com sucesso;

        public class Main {

    public static void main(String[] args) {
	    // write your code here
	    System.out.println("Hello World!");
	    
    }
}
        
        
    
  + Algoritmo de ordenação [quicksort](https://en.wikipedia.org/wiki/Sorting_algorithm#Quicksort);
    
   
      public class QuickSort {
       
    int partition(int arr[], int low, int high) 
    { 
        int pivot = arr[high];  
        int i = (low-1); // index of smaller element 
        for (int j=low; j<high; j++) 
        { 
            // If current element is smaller than or 
            // equal to pivot 
            if (arr[j] <= pivot) 
            { 
                i++; 
  
                // swap arr[i] and arr[j] 
                int temp = arr[i]; 
                arr[i] = arr[j]; 
                arr[j] = temp; 
            } 
        } 
  
        // swap arr[i+1] and arr[high] (or pivot) 
        int temp = arr[i+1]; 
        arr[i+1] = arr[high]; 
        arr[high] = temp; 
  
        return i+1; 
    } 
  
 
    void sort(int arr[], int low, int high) 
    { 
        if (low < high) 
        { 

            int pi = partition(arr, low, high); 
   
            sort(arr, low, pi-1); 
            sort(arr, pi+1, high); 
        } 
    } 

static void printArray(int arr[]) 
    { 
        int n = arr.length; 
        for (int i=0; i<n; ++i) 
            System.out.print(arr[i]+" "); 
        System.out.println(); 
    } 
  
    public static void main(String args[]) 
    { 
        int arr[] = {10, 7, 8, 9, 1, 5}; 
        int n = arr.length; 
  
        QuickSort ob = new QuickSort(); 
        ob.sort(arr, 0, n-1); 
  
        System.out.println("sorted array"); 
        printArray(arr); 
    } 
} 
      
      
  + Função Ackerman: O programa que resolve o problema deve imprimir o resultado da função de Ackermann simplificada corretamente:
<p>
<a href="https://www.codecogs.com/eqnedit.php?latex=A(m,&space;n)&space;=&space;
\begin{cases}&space;n&plus;1&space;&&space;\mbox{if&space;}&space;m&space;=&space;0&space;
\\&space;A(m-1,&space;1)&space;&&space;\mbox{if&space;}&space;m&space;>&space;0&space;\&space;
\mbox{&space;and&space;}&space;n&space;=&space;0&space;\\&space;A(m-1,&space;A(m,&space;n-1))&space;&&space;
\mbox{if&space;}&space;m&space;>&space;0&space;\mbox{&space;and&space;}&space;n&space;>&space;0.&space;
\end{cases}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?A(m,&space;n)&space;=&space;\begin{cases}&space;n&plus;1&space;&&space;\mbox{if&space;}&space;m&space;=&space;0&space;\\&space;A(m-1,&space;1)&space;&&space;\mbox{if&space;}&space;m&space;>&space;0&space;\&space;\mbox{&space;and&space;}&space;n&space;=&space;0&space;\\&space;A(m-1,&space;A(m,&space;n-1))&space;&&space;\mbox{if&space;}&space;m&space;>&space;0&space;\mbox{&space;and&space;}&space;n&space;>&space;0.&space;\end{cases}" title="A(m, n) = \begin{cases} n+1 & \mbox{if } m = 0 \\ A(m-1, 1) & \mbox{if } m > 0 \ \mbox{ and } n = 0 \\ A(m-1, A(m, n-1)) & \mbox{if } m > 0 \mbox{ and } n > 0. \end{cases}" /></a>
</p>  


Além disso, apresente quais as principais [IDEs](https://en.wikipedia.org/wiki/Integrated_development_environment) para a linguagem escolhida.

    
        Netbeans
        Itellij
        Eclipse
        