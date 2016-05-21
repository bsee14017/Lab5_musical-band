# Nabeela
#include<conio.h>
#include<stdio.h>
#include<string>
using namespace std;
class Band
{
	public:
		Band()
		{
			 count=0;
		}
	protected:
		int count;
		virtual int getcount();
		virtual void add_pyro_technician();
		virtual void Remove_pyro_technician();
		
		
		
};
 class Jazz:Band
 {
 	public:
 		int getcount()
		{
			return count;
		}
 		
 };
 
 class metal:Band
 {
 	public:
 		metal()
 		{
 			
		}
		int getcount()
		{
			return count;
		}
		void add_pyro_technician()
		{
			count++;
		}
		void Remove_pyro_technician()
		{
			count--;
		}

		
 	
 };
 
 class symphony:Band
 {
 		private:
	 	string name;
 	public:
 		
 		int getcount()
		{
			return count;
		}
 		string get_name()
 		{
 			return name;
		}
 		void set_name(string n )
 		{
 			name=n;
		}
 
 };





int main ()
{
	

	metal j;
	j.add_pyro_technician();
	j.getcount();
	j.Remove_pyro_technician();
}
