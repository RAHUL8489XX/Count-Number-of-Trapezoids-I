# Count-Number-of-Trapezoids-I  
Link: https://leetcode.com/contest/weekly-contest-459/problems/count-number-of-trapezoids-i/description/

You are given a 2D integer array points, where points[i] = [xi, yi] represents the coordinates of the ith point on the Cartesian plane.

A horizontal trapezoid is a convex quadrilateral with at least one pair of horizontal sides (i.e. parallel to the x-axis). Two lines are parallel if and only if they have the same slope.

Return the number of unique horizontal trapezoids that can be formed by choosing any four distinct points from points.

Since the answer may be very large, return it modulo 109 + 7.

Note: Please do not copy the description during the contest to maintain the integrity of your submissions.



💡 Key Insight
To form horizontal trapezoids:

You need two points with the same y-value on one horizontal line.

And two other points on a different horizontal line (also same y-value).

This means:

Group all points by y coordinate.

For each pair of horizontal lines, count how many ways you can pick 2 points from each line.

Multiply the combinations: C(n₁, 2) * C(n₂, 2).
