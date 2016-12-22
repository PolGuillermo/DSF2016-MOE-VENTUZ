# DSF - Tile Game (MOE 2016) VENTUZ C# CODE

# Requirements

- Ventuz Designer 

# Instructions

Input fileds 
  - coupon
  - score

Input filed for Request Actions (Value: 0 or 1)
  - randomRequest
  - validationRequest
  - gameendRequest

Outputs
  - multiplechoice
  - question
  - valresult
  
  
# Random Image & Multiple Choice
 
Place the code below inside "public override void Validate() {"

	// When value chage to 1 activate request
	if(this.randomRequest == 1)
	{
		this.question = randomnumber(1, 51);
		this.multiplechoice = randomaswer();
		changed = true;
	}
 


