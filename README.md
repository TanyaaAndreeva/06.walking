# 06.walking
task 06. Walking from Exe 05
internal class Program
    {
        static void Main(string[] args)
        {
            int stepsGoal = 10000;

            int totalSteps = 0;

            while ( totalSteps < stepsGoal)
            {
                string input= Console.ReadLine();

                if(input == "Going home")
                {
                   int stepsToHome= int.Parse(Console.ReadLine());

                    totalSteps += stepsToHome;

                    int diff = stepsGoal - totalSteps;

                    if (totalSteps < stepsGoal)
                    {
                        Console.WriteLine($"{diff} more steps to reach goal.");
                    }
                }
                else
                {
                    
                        int steps = int.Parse(input);
                    totalSteps += steps;

                    if(totalSteps >= stepsGoal)
                        {
                        int exceededSteps = totalSteps - stepsGoal; 
                        Console.WriteLine($"Goal reached! Good job!");
                        Console.WriteLine($"{exceededSteps} steps over the goal!");
                        break;
                    }
                    

                    
                }
               
            }

            

            
            
        }
    }
}
