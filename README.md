#Home work
@Throws(IllegalArgumentException::class)
fun minOfVarArg(vararg list:Int):Int  {
    if (list.isEmpty()) {
        throw IllegalArgumentException
    }
    var min = list[0]
    for (i in list) {
        if (i < min) {
            min = i
        }
    }
    return min
}

#home work
class Engineer (val name: String, val department: String)

class QA(name: String, department: String):Engineer(name, department){
    override fun toString(): String {
        return "name : " + this.name + " department: " + this.department
    }

   @Throws(Exception::class)
    fun realiseTesting(dayToRelease: Int, newFunc: ArrayList<String>): Boolean {
        val tasksInDay = 10
        val countTasks = newFunc.size
                if (dayToRelease > 20) {
            throw IllegalArgumentException
        }
        val tasksCompletedBeforeRelease = tasksInDay * dayToRelease
        return countTasks <= tasksCompletedBeforeRelease
    }
}

