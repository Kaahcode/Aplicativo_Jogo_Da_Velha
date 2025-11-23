
            if (
             (btn10.Text == "X" && btn11.Text == "X" && btn12.Text == "X") ||
            (btn13.Text == "X" && btn14.Text == "X" && btn15.Text == "X") ||
            (btn16.Text == "X" && btn17.Text == "X" && btn18.Text == "X") ||

         // Coluna
         (btn10.Text == "X" && btn13.Text == "X" && btn16.Text == "X") ||
         (btn11.Text == "X" && btn14.Text == "X" && btn17.Text == "X") ||
         (btn12.Text == "X" && btn15.Text == "X" && btn18.Text == "X") ||

         // Diagonal
         (btn10.Text == "X" && btn14.Text == "X" && btn18.Text == "X") ||
         (btn12.Text == "X" && btn14.Text == "X" && btn16.Text == "X")
         )

            {
                DisplayAlert("Parabéns!", " X ganhou!", "OK");
                Zerar();
                return;

            }
            if (
             (btn10.Text == "O" && btn11.Text == "O" && btn12.Text == "O") ||
             (btn13.Text == "O" && btn14.Text == "O" && btn15.Text == "O") ||
             (btn16.Text == "O" && btn17.Text == "O" && btn18.Text == "O") ||

             // Coluna
             (btn10.Text == "O" && btn13.Text == "O" && btn16.Text == "O") ||
             (btn11.Text == "O" && btn14.Text == "O" && btn17.Text == "O") ||
             (btn12.Text == "O" && btn15.Text == "O" && btn18.Text == "O") ||

             // Diagonal
             (btn10.Text == "O" && btn14.Text == "O" && btn18.Text == "O") ||
             (btn12.Text == "O" && btn14.Text == "O" && btn16.Text == "O")
             )

            {
                DisplayAlert("Parabéns!", "O ganhou!", "OK");
                Zerar();
                return;

            }
            if (
              btn10.Text == "" && btn11.Text == "" && btn12.Text == "" &&
              btn13.Text == "" && btn14.Text == "" && btn15.Text == "" &&
              btn16.Text == "" && btn17.Text == "" && btn18.Text == ""
          )
            {
                DisplayAlert("Deu velha!", "Ninguém ganhou!", "OK");
                Zerar();
                return;
            }

        }//Fecha método

        void Zerar()
        {
            btn10.Text = "";
            btn11.Text = "";
            btn12.Text = "";
            btn13.Text = "";
            btn14.Text = "";
            btn15.Text = "";      
            btn16.Text = "";
            btn17.Text = "";
            btn18.Text = "";

            btn10.IsEnabled = true;
            btn11.IsEnabled = true;
            btn12.IsEnabled = true;
            btn13.IsEnabled = true;
            btn14.IsEnabled = true;
            btn15.IsEnabled = true;
            btn16.IsEnabled = true;
            btn17.IsEnabled = true;
            btn18.IsEnabled = true;

        }
    } // Fecha classe
}//Fecha namespace
