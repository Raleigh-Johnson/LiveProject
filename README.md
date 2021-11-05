# C\#LiveProject
This is a summary of the things I learned through the live project and how I can apply them to my work ethic.


The C\# Live project was a very good experience for me, both in a professional sense, and a personal sense. 
Getting an idea of what workflow in a real office space might be like is invaluable to one's success. 

# Crud Pages
I worked in the "Production" side of the group and worked on CRUD pages, designing said pages, and working with databases. 
My "CastMembers folder was a fairly easy one, mostly just instantating variables and giving them datatypes:

# Crud Pages CastMembers.cs
namespace TheatreCMS3.Areas.Prod.Models
{
    public enum PositionEnum
    {
        Actor,
        Director,
        StageManager,
        Technician,
        Other
    }
    public class CastMember
    {
        public int CastMemberId { get; set; }
        public string Name { get; set; }
        public int? YearJoined { get; set; }
        public PositionEnum MainRole { get; set; }
        public string Bio { get; set; }
        public bool CurrentMember { get; set; }
        public string Character { get; set; }
        public int? CastYearLeft { get; set; }
        public int? DebutYear { get; set; }
    }
}
