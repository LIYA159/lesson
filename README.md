# lesson


В массиве задана программа для
черепашки (команды зашифрованы: 1- вперед 10; 2 – назад 10; 3 – поворот направо
на 90 градусов: 4 – поворот налево на 90 градусов). Необходимо исполнить данную
программу и получить на экране соответствующий рисунок

{
            Turtle.Show();
            Turtle.Speed = 10;
            GraphicsWindow.PenColor = GraphicsWindow.GetRandomColor();
            int n = int.Parse(Console.ReadLine());
            int[] a = new int[n];
            Random rnd = new Random();
            for (int i=0;i<a.Length ; i++)
            {
                a[i] = rnd.Next(1, 5);
                Console.Write(a[i]);
            }
                for (int i = 0; i < a.Length; i++)
                {
                    switch (a[i])
                    {
                        case 1 :Turtle.Move(20);break;
                        case 2 : Turtle.Move(-20); break;
                        case 3 : Turtle.TurnRight(); break;
                        case 4 : Turtle.TurnLeft(); break;
                    }
                }

