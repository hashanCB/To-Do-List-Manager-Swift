import UIKit

struct Task {
    var title : String
    var description : String
    var dueDate : Date?
    var priority : priority
    var completed : String
}
enum priority : String {
    case high ,medium ,low
}
class TaskManager {
    
    var Tasks : [Task] = []
    
    func addtask (on addTasks : Task ){
        Tasks.append(addTasks)
    }
     
    func displaytask (){
        
        for i in Tasks {
            print( "Title namw \(i.title) , description : \(i.description) , Iscompted \(i.completed)")
        }
    }
    
    func markasComp (on index : Int){
        if(index >= 0 && index <= Tasks.count){
            Tasks[index].completed  = "Yes"
        } }
    
    func filercatlog (on compted : String? = nil , by piority : priority? = nil) -> [Task]{
        
        var Filtertask = Tasks
        
//        if compted == "Yes" {
//            Filtertask.filter { $0.completed == "Yes" }
//        }
//        
        switch compted {
        case "Yes" :
           print ( Filtertask.filter { $0.completed == "Yes"} )
        case "No" :
            print (Filtertask.filter{ $0.completed == "No"} )
        default :
            print ("Valid Not Input")
               }
        
        
        return Filtertask
    }
    
    func shorting (on shorting : String) {
        
        var sortArray = Tasks
        
        switch shorting {
        case "piority" :
            sortArray.sort  {$0.priority.rawValue < $1.priority.rawValue}
        case "dueDate" :
        print("hello")
        default :
            break
        }
        
      
    }
}


var TaskLog = TaskManager()

var task1 = Task(title: "Hashan1", description: "Hashan", priority: .medium , completed: "No")
var task2 = Task(title: "Hashan2", description: "Hashan", priority: .low , completed: "No")
var task3 = Task(title: "Hashan3", description: "Hashan", priority: .high , completed: "Yes")

TaskLog.addtask(on: task1)
TaskLog.addtask(on: task2)
TaskLog.addtask(on: task3)
//TaskLog.displaytask()
//TaskLog.markasComp(on: 0)
//TaskLog.displaytask()
//var newtray = TaskLog.filercatlog(on: "No")
//
//for i in newtray {
//    print( "Title namw \(i.title) , description : \(i.description) , Iscompted \(i.completed)")
//}

var newsarray = TaskLog.shorting(on: "piority")
for i in newsarray{
    print( "Title namw \(i.title) , description : \(i.description) , Iscompted \(i.completed)")
}
