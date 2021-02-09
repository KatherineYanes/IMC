using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace WindowsFormsApp6
{
    public partial class Form1 : Form

    {
        
        public Form1()
        {
            InitializeComponent();
        }

        private void label2_Click(object sender, EventArgs e)
        {

        }

        private void button1_Click(object sender, EventArgs e)
        {

            double i, a, p;
            a = double.Parse(textBox1.Text);
            p = double.Parse(textBox2.Text);
            i = p / (a * a);
            MessageBox.Show("su IMC es " + i, "IMC", MessageBoxButtons.OK);

            if (i < 18)
            {
                MessageBox.Show("Bajo peso", "usted tiene:", MessageBoxButtons.OK);
            }
            else if (i < 25)
            {

                MessageBox.Show("Peso normal", "usted tiene:", MessageBoxButtons.OK);


            }
            else if (i < 30)
            {
                MessageBox.Show("sobre peso", "usted tiene:", MessageBoxButtons.OK);

            }
            else
            {

                MessageBox.Show("Obesidad", "usted tiene:", MessageBoxButtons.OK);
            }


        }

        

        private void button2_Click(object sender, EventArgs e)
        {
            Application.Exit();
        }

        private void button3_Click(object sender, EventArgs e)
        {
            textBox1.Clear();
            textBox2.Clear();
            
        }

      

        
    }
}
