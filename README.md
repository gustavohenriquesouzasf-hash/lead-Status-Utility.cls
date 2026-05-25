public class LeadUtility {
    public static void viewStatus(){
        list<Lead> leadList = [SELECT Name, Status FROM Lead];
        for(Lead ld : leadList){
            String ledSta = ld.Name + ' : ' + ld.Status; 
            system.debug(ledSta);
        }
    }
}
