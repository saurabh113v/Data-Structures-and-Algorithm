class Solution {
    public double angleClock(int hour, int minutes) {
        // Calculate the angle of the hour hand from 12 o'clock position
        // Hour hand moves 30 degrees per hour (360° / 12 hours = 30°)
        // Hour hand also moves 0.5 degrees per minute (30° / 60 minutes = 0.5°)
        double hourAngle = 30.0 * hour + 0.5 * minutes;
      
        // Calculate the angle of the minute hand from 12 o'clock position
        // Minute hand moves 6 degrees per minute (360° / 60 minutes = 6°)
        double minuteAngle = 6.0 * minutes;
      
        // Calculate the absolute difference between the two angles
        double angleDifference = Math.abs(hourAngle - minuteAngle);
      
        // Return the smaller angle between the two possible angles
        // The angle can be measured clockwise or counter-clockwise
        return Math.min(angleDifference, 360.0 - angleDifference);
    }
}
