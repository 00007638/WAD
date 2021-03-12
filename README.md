using System.ComponentModel.DataAnnotations;  
  
namespace RestarauntLogin.Models  
{  
    public class CBUserModel  
    {  
        [Required(ErrorMessage = "UserName is required")]  
        public string UserName { get; set; }  
        [Required(ErrorMessage = "Password is required")]  
        [DataType(DataType.Password)]  
        public string Password { get; set; }  
    }  
}  

-----------------------------------------------------------
using System;  
using System.Collections.Generic;  
using System.Linq;  
using System.Threading.Tasks;  
using System.ComponentModel.DataAnnotations;  
  
namespace WaiterRegistration.Models  
{  
    public class Waiter
    {  
        [Key]  
        public int UserId { get; set; }  
  
        [Required(ErrorMessage ="Please Enter Name..")]  
        [Display(Name = "UserName")]  
        public string name { get; set; }  
  
        [Required(ErrorMessage ="Please Enter Password...")]  
        [DataType(DataType.Password)]  
        [Display(Name ="Password")]  
        public string password { get; set; }  
  
        [Required(ErrorMessage = "Please Enter the Confirm Password...")]  
        [DataType(DataType.Password)]  
        [Display(Name = "Confirm Password")]  
        [Compare("Pwd")]  
        public string ConfirmPassword { get; set; }  
  
        [Required(ErrorMessage = "Please Enter Email...")]  
        [Display(Name = "Email")]  
        public string Email { get; set; }  
  
        [Required(ErrorMessage = "Please enter date of birth...")]  
        [Display(Name = "Date of birth")]  
        public date type Dbo { get; set; }  
  
        [Required(ErrorMessage = "Please enter unique number...")]  
        [Display(Name = "Unique number")]  
        public int UniqueNumber { get; set; }  
  
  
    }  
}  
