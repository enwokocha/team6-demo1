pipeline{
    agent any
    stages('1-test-git'){
        steps{
            echo "unit testing"
        }
    }
    stages('2-build'){
        steps{
            echo "building...."
        }
    }
    stages('3-pr-test'){
        steps{
            echo "testing...."
        }
    }
}
