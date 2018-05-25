problem statement:
	reverse the given string

prep steps:
	paramenters: a string
	return: string, reversed
	test cases: Test.expect(solution('world') == 'dlrow')
	steps:
		split string into array 
			- domain transfer for maniuplabiliity
		reverse array
		convert back to string
			- back to domain


implementation:
	
	1.   empty function
		function solution(string) {
			let reversed_string = "";

			return reversed_string;
		}

	2.   split into an array
		function solution(string) {
			let reversed_string = "";
			let temp_array = [];

			temp_array = string.split("");


			return reversed_string;
		}


	3.a  reverse the array with native method
		function solution(string) {
		    let reversed_string = "";
		    let temp_array = [];
		    
		    temp_array = string.split("");
		    temp_array = temp_array.reverse();
		    
		    return reversed_string;
		};

	3.b  reverse the array with control flow
		function solution(string) {
		    let reversed_string = "";
		    let temp_array = [];
		    let reversed_temp = [];
		    
		    temp_array = string.split("");
		    for (let index = string.length; index < 0; index--) {
		    	reversed_temp.push(temp_array[index]);
		    };

		    
		    return reversed_string;
		};

	4.   convert the array back to string with strategy a
		function solution(string) {
		    let reversed_string = "";
		    let temp_array = [];
		    
		    temp_array = string.split("");
		    temp_array = temp_array.reverse();
		    reversed_string = temp_array.join("");
		    
		    return reversed_string;
		}; 


components analysis:
	variables:
		reversed_string 
			purpose: a string, used to build up our return value
			initialized: empty
			end: the argument backwards
		temp_array
			purpose: an array used to more conveniently manipulate the letters. 
			initialized: empty 
			end: with all the letters in reverse
	features:
		data structure - array: because they can easily manipulate ordered elements

behavior breakdown:
	- write extra examples of each
	string.split:
	temp_array.reverse:
	temp_array.join:
























