<script setup lang="ts">
import {
  Activity,
  ArrowUpRight,
  CircleUser,
  CreditCard,
  DollarSign,
  Menu,
  Package2,
  Search,
  Users,
} from "lucide-vue-next";
</script>

<template>
  <div class="grid gap-4 md:grid-cols-2 md:gap-8 lg:grid-cols-4">
    <CardThings />
    <ActivityCard />
  </div>
  <div class="grid gap-4 md:gap-8 lg:grid-cols-2 xl:grid-cols-3">
    <Card class="xl:col-span-2">
      <CardHeader class="flex flex-row items-center">
        <div class="grid gap-2">
          <CardTitle>Transactions</CardTitle>
          <CardDescription>
            Recent transactions from your store.
          </CardDescription>
        </div>
        <Button as-child size="sm" class="ml-auto gap-1">
          <a href="#">
            View All
            <ArrowUpRight class="h-4 w-4" />
          </a>
        </Button>
      </CardHeader>
      <CardContent>
        <Table>
          <TableHeader>
            <TableRow>
              <TableHead>Customer</TableHead>
              <TableHead class="hidden xl:table-column"> Type </TableHead>
              <TableHead class="hidden xl:table-column"> Status </TableHead>
              <TableHead class="hidden xl:table-column"> Date </TableHead>
              <TableHead class="text-right"> Amount </TableHead>
            </TableRow>
          </TableHeader>
          <TableBody>
            <TableRow>
              <TableCell>
                <div class="font-medium">Liam Johnson</div>
                <div class="hidden text-sm text-muted-foreground md:inline">
                  liam@example.com
                </div>
              </TableCell>
              <TableCell class="hidden xl:table-column"> Sale </TableCell>
              <TableCell class="hidden xl:table-column">
                <Badge class="text-xs" variant="outline"> Approved </Badge>
              </TableCell>
              <TableCell class="hidden md:table-cell lg:hidden xl:table-column">
                2023-06-23
              </TableCell>
              <TableCell class="text-right"> $250.00 </TableCell>
            </TableRow>
            <TableRow>
              <TableCell>
                <div class="font-medium">Olivia Smith</div>
                <div class="hidden text-sm text-muted-foreground md:inline">
                  olivia@example.com
                </div>
              </TableCell>
              <TableCell class="hidden xl:table-column"> Refund </TableCell>
              <TableCell class="hidden xl:table-column">
                <Badge class="text-xs" variant="outline"> Declined </Badge>
              </TableCell>
              <TableCell class="hidden md:table-cell lg:hidden xl:table-column">
                2023-06-24
              </TableCell>
              <TableCell class="text-right"> $150.00 </TableCell>
            </TableRow>
            <TableRow>
              <TableCell>
                <div class="font-medium">Noah Williams</div>
                <div class="hidden text-sm text-muted-foreground md:inline">
                  noah@example.com
                </div>
              </TableCell>
              <TableCell class="hidden xl:table-column">
                Subscription
              </TableCell>
              <TableCell class="hidden xl:table-column">
                <Badge class="text-xs" variant="outline"> Approved </Badge>
              </TableCell>
              <TableCell class="hidden md:table-cell lg:hidden xl:table-column">
                2023-06-25
              </TableCell>
              <TableCell class="text-right"> $350.00 </TableCell>
            </TableRow>
            <TableRow>
              <TableCell>
                <div class="font-medium">Emma Brown</div>
                <div class="hidden text-sm text-muted-foreground md:inline">
                  emma@example.com
                </div>
              </TableCell>
              <TableCell class="hidden xl:table-column"> Sale </TableCell>
              <TableCell class="hidden xl:table-column">
                <Badge class="text-xs" variant="outline"> Approved </Badge>
              </TableCell>
              <TableCell class="hidden md:table-cell lg:hidden xl:table-column">
                2023-06-26
              </TableCell>
              <TableCell class="text-right"> $450.00 </TableCell>
            </TableRow>
            <TableRow>
              <TableCell>
                <div class="font-medium">Liam Johnson</div>
                <div class="hidden text-sm text-muted-foreground md:inline">
                  liam@example.com
                </div>
              </TableCell>
              <TableCell class="hidden xl:table-column"> Sale </TableCell>
              <TableCell class="hidden xl:table-column">
                <Badge class="text-xs" variant="outline"> Approved </Badge>
              </TableCell>
              <TableCell class="hidden md:table-cell lg:hidden xl:table-column">
                2023-06-27
              </TableCell>
              <TableCell class="text-right"> $550.00 </TableCell>
            </TableRow>
          </TableBody>
        </Table>
      </CardContent>
    </Card>
    <Card>
      <CardHeader>
        <CardTitle>Recent Sales</CardTitle>
      </CardHeader>
      <CardContent class="grid gap-8">
        <div class="flex items-center gap-4">
          <Avatar class="hidden h-9 w-9 sm:flex">
            <AvatarImage src="" alt="Avatar" />
            <AvatarFallback>OM</AvatarFallback>
          </Avatar>
          <div class="grid gap-1">
            <p class="text-sm font-medium leading-none">Olivia Martin</p>
            <p class="text-sm text-muted-foreground">olivia.martin@email.com</p>
          </div>
          <div class="ml-auto font-medium">+$1,999.00</div>
        </div>
        <div class="flex items-center gap-4">
          <Avatar class="hidden h-9 w-9 sm:flex">
            <AvatarImage src="" alt="Avatar" />
            <AvatarFallback>JL</AvatarFallback>
          </Avatar>
          <div class="grid gap-1">
            <p class="text-sm font-medium leading-none">Jackson Lee</p>
            <p class="text-sm text-muted-foreground">jackson.lee@email.com</p>
          </div>
          <div class="ml-auto font-medium">+$39.00</div>
        </div>
        <div class="flex items-center gap-4">
          <Avatar class="hidden h-9 w-9 sm:flex">
            <AvatarImage src="" alt="Avatar" />
            <AvatarFallback>IN</AvatarFallback>
          </Avatar>
          <div class="grid gap-1">
            <p class="text-sm font-medium leading-none">Isabella Nguyen</p>
            <p class="text-sm text-muted-foreground">
              isabella.nguyen@email.com
            </p>
          </div>
          <div class="ml-auto font-medium">+$299.00</div>
        </div>
        <div class="flex items-center gap-4">
          <Avatar class="hidden h-9 w-9 sm:flex">
            <AvatarImage src="" alt="Avatar" />
            <AvatarFallback>WK</AvatarFallback>
          </Avatar>
          <div class="grid gap-1">
            <p class="text-sm font-medium leading-none">William Kim</p>
            <p class="text-sm text-muted-foreground">will@email.com</p>
          </div>
          <div class="ml-auto font-medium">+$99.00</div>
        </div>
        <div class="flex items-center gap-4">
          <Avatar class="hidden h-9 w-9 sm:flex">
            <AvatarImage src="" alt="Avatar" />
            <AvatarFallback>SD</AvatarFallback>
          </Avatar>
          <div class="grid gap-1">
            <p class="text-sm font-medium leading-none">Sofia Davis</p>
            <p class="text-sm text-muted-foreground">sofia.davis@email.com</p>
          </div>
          <div class="ml-auto font-medium">+$39.00</div>
        </div>
      </CardContent>
    </Card>
  </div>
</template>
